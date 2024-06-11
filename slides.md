---
# try also 'default' to start simple
theme: seriph
zoom: 1.5
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# background: https://cover.sli.dev
# some information about your slides, markdown enabled
title: Welcome to Slidev
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply any unocss classes to the current slide
class: text-center
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# https://sli.dev/guide/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/guide/syntax#mdc-syntax
mdc: true
fonts:
  # like font-family in css, you can use `,` to separate multiple fonts for fallback
  sans: 'Vazirmatn NL,Segoe UI'
  # mark 'Helvetica Neue' as local font
  local: Helvetica Neue
  mono: Consolas

# htmlAttrs:
#   dir: rtl
#   lang: fa
---


به نام خدا

# TypeScript
شهاب‌الدّین موحّدی،
سیدمحمّد پرهام ابوالقاسمی،
حمیدرضا میخچی


---

# مقدمه‌ای بر تایپ‌اسکریپت
<div dir="rtl">

تایپ‌اسکریپت یک زبان برنامه‌نویسی است که بر روی جاوااسکریپت ساخته شده و ویژگی‌های بیشتری به آن اضافه می‌کند. این زبان به توسعه‌دهندگان کمک می‌کند تا کدهای قابل نگهداری و بدون خطا بنویسند.

</div>

---

# نصب تایپ‌اسکریپت
<div dir="rtl">

برای نصب تایپ‌اسکریپت می‌توانید از npm استفاده کنید:

</div>

```bash
npm install -g typescript
```

<div dir="rtl">

برای بررسی نصب تایپ‌اسکریپت می‌توانید از دستور زیر استفاده کنید:

</div>

```bash
tsc --version
```

---

# اولین برنامه تایپ‌اسکریپت
<div dir="rtl">

یک فایل جدید با پسوند `.ts` ایجاد کنید و کد زیر را در آن بنویسید:

</div>

```typescript {monaco-run}
function greet(name: string): string {
    return `Hello, ${name}!`;
}

let user = 'TypeScript';
console.log(greet(user));
```

<div dir="rtl">

برای کامپایل کردن کد تایپ‌اسکریپت به جاوااسکریپت از دستور زیر استفاده کنید:

</div>

```bash
tsc filename.ts
```

---

# تایپ‌ها در تایپ‌اسکریپت
<div dir="rtl">

تایپ‌اسکریپت انواع مختلفی از تایپ‌ها را پشتیبانی می‌کند که شامل primitive types، arrays، tuples و enum می‌باشد.

</div>

```typescript {monaco-run}
let isDone: boolean = false;
let decimal: number = 6;
let color: string = "blue";
let list: number[] = [1, 2, 3];
let tuple: [string, number] = ["hello", 10];

enum Color {
    Red,
    Green,
    Blue
}
let c: Color = Color.Green;
```

---

# اینترفیس‌ها در تایپ‌اسکریپت
<div dir="rtl">

اینترفیس‌ها برای تعریف ساختارهای داده‌ای مورد استفاده قرار می‌گیرند.

</div>

```typescript {monaco-run}
interface Person {
    firstName: string;
    lastName: string;
}

function greeter(person: Person) {
    return `Hello, ${person.firstName} ${person.lastName}`;
}

let user = { firstName: "John", lastName: "Doe" };
console.log(greeter(user));
```

---

# کلاس‌ها در تایپ‌اسکریپت
<div dir="rtl">

کلاس‌ها در تایپ‌اسکریپت مشابه کلاس‌ها در دیگر زبان‌های شی‌گرا هستند.

</div>

```typescript {monaco-run}
class Greeter {
    greeting: string;

    constructor(message: string) {
        this.greeting = message;
    }

    greet() {
        return `Hello, ${this.greeting}`;
    }
}

let greeter = new Greeter("world");
console.log(greeter.greet());
```

---

<div dir="rtl">

تایپ‌اسکریپت ابزار قدرتمندی است که با افزودن تایپ‌ها به جاوااسکریپت، توسعه نرم‌افزارهای بزرگ و پیچیده را آسان‌تر می‌کند. با یادگیری و استفاده از تایپ‌اسکریپت می‌توانید کدهای قابل نگهداری‌تر و بدون خطاتری بنویسید.

</div>
