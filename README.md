# پروژه پایانی کارشناسی: مقایسه عملکرد Docker و Podman

![Container Technologies](https://img.shields.io/badge/tech-Docker%20%26%20Podman-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-Completed-brightgreen)

**دانشگاه شهید مدنی آذربایجان**  
**دانشکده مهندسی کامپیوتر**  

## فهرست مطالب
- [معرفی پروژه](#معرفی-پروژه)
- [اهداف پروژه](#اهداف-پروژه)
- [فناوری‌های استفاده شده](#فناوری‌های-استفاده-شده)
- [نحوه اجرا](#نحوه-اجرا)
- [ساختار پروژه](#ساختار-پروژه)
- [نتایج کلیدی](#نتایج-کلیدی)
- [مشارکت](#مشارکت)
- [مجوز](#مجوز)
- [تماس](#تماس)

## معرفی پروژه
این پروژه به عنوان پروژه پایانی کارشناسی مهندسی کامپیوتر با هدف مقایسه عملکرد دو پلتفرم کانتینرسازی **Docker** و **Podman** طراحی و اجرا شده است.

![مقایسه عملکرد](docs/comparison-chart.png)

## اهداف پروژه
- 🎯 مقایسه مصرف منابع CPU و حافظه
- 🎯 ارزیابی عملکرد شبکه در سناریوهای مختلف
- 🎯 سنجش زمان راه‌اندازی کانتینرها
- 🎯 بررسی امنیت و قابلیت‌های مدیریتی

## فناوری‌های استفاده شده
### پلتفرم‌ها
- Docker 24.0.5
- Podman 4.2.0
- Kubernetes (برای تست‌های تکمیلی)

### ابزارهای تست
| ابزار | نسخه | کاربرد |
|-------|------|--------|
| sysbench | 1.0.20 | تست عملکرد CPU و حافظه |
| stress-ng | 0.13.10 | ایجاد بار کاری |
| htop | 3.0.5 | مانیتورینگ منابع |
| iperf3 | 3.10.1 | تست عملکرد شبکه |

## نحوه اجرا
### پیش‌نیازها
- سیستم عامل: Ubuntu 22.04 LTS
- حداقل سخت‌افزار:
  - 4GB RAM
  - 2 هسته CPU
  - 20GB فضای ذخیره‌سازی

### دستورات نصب
```bash
# نصب پیش‌نیازها
sudo apt update && sudo apt install -y \
    docker.io \
    podman \
    sysbench \
    stress-ng \
    htop \
    iperf3

اجرای تست‌ها
# کلون کردن ریپوزیتوری
git clone https://github.com/yourusername/docker-podman-benchmark.git

# تغییر مسیر به دایرکتوری پروژه
cd docker-podman-benchmark

# اجرای اسکریپت اصلی
chmod +x run_benchmarks.sh
./run_benchmarks.sh

ساختار پروژه
├── .github/            # تنظیمات CI/CD
├── docs/               # مستندات پروژه
│   ├── proposal.pdf    # پروپوزال اولیه
│   ├── report.pdf      # گزارش نهایی
│   └── slides/         # ارائه دفاع
├── src/                # کدهای اجرایی
│   ├── benchmarks/     # اسکریپت‌های تست
│   ├── monitoring/     # ابزارهای مانیتورینگ
│   └── analysis/       # کدهای تحلیل داده
├── data/               # داده‌های خام
│   ├── docker/         # نتایج Docker
│   └── podman/         # نتایج Podman
└── README.md           # همین فایل

نتایج کلیدی
مقایسه عملکرد CPU



معیار
Docker
Podman



سرعت پردازش (event/sec)
458.84
452.91


تأخیر متوسط (ms)
2.18
2.21


مقایسه مصرف حافظه

مشارکت
پروژه به صورت متن‌باز ارائه شده و مشارکت‌پذیر است:

ریپوزیتوری را Fork کنید
شاخه جدید ایجاد کنید (git checkout -b feature/your-feature)
تغییرات را Commit کنید (git commit -m 'Add some feature')
به شاخه اصلی Push کنید (git push origin feature/your-feature)
Pull Request باز کنید

تماس
محمد مهدی رسول امینی📧 ایمیل: mohamadmahdiamini122@gmail.com🔗 لینکدین: https://www.linkedin.com/in/mohammadmahdirasoulamini/🐦
  
    
  
  
    
  

```
