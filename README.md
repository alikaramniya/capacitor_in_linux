# capacitor_in_linux

### حل کردن مشگل CAPACITOR_ANDROID_STUDIO_PATH در آرچ لینوکس

#### اول از همه باید دستور پایین رو اجرا کنیم تا بفهمیم که android-studio توی چه مسیری نصب شده است پس دستور پایین رو اجرا میکنیم

```
whereis studio.sh
```

#### که خروجیش مقدار رو باید کپی کنید که چیزی شبیه یا خود ادرس پایین رو بهت میده

```
/opt/android-studio/bin/studio.sh
```

#### بعد از کپی کردن ادرس برین توی فایل .zshrc و کد پایین رو قرار بدین

```
export CAPACITOR_ANDROID_STUDIO_PATH="/opt/android-studio/bin/studio.sh"
```

#### بعد دستور پایین رو اجرا میکنیم 

```
source ~/.zshrc
```

#### الان کافیه بریم توی مسیر سایت یا پروژه و دستور پایین رو اجرا کنیم میاد پروژه رو برامون با استفاده از android-studio باز میکنه

```
npx cap open android
```
