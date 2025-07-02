<h1>اجرای storybook در زیرساخت</h1>

<h4>
⬇️ ۱. ابتدا باید نسخه‌ی Node.js را به ۱۸ تغییر دهید.
برای این کار می‌توانید از ابزار nvm (Node Version Manager) استفاده کنید.
</h4>

<h5>
مراحل نصب و استفاده از nvm مطابق با داکیومنت سایت nodejs.org:
</h5>

<h3>
📥 دانلود و نصب nvm:
</h3>

<h4>
(بهتر است برای به‌روز بودن به سایت nodejs.org مراجعه کنید)
</h4>

<pre align="left">
<code dir="ltr">
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.3/install.sh | bash
</code>
</pre>

<h3>
🚀 فعال‌سازی nvm در ترمینال فعلی:
</h3>

<pre align="left">
<code dir="ltr">source "$HOME/.nvm/nvm.sh"</code>
</pre>

<h3>
📦 نصب نسخه‌ی ۱۸ از Node.js:
</h3>
<pre align="left">
<code dir="ltr">nvm install 18</code>
</pre>

<h3>
⚙️ استفاده از نسخه‌ی ۱۸:
</h3>

<pre align="left">
<code dir="ltr">nvm use 18</code>
</pre>

<h4>
 📂 ۲. پس از تنظیم نسخه‌ی Node، لازم است پوشه‌های node_modules و
package-lock.json را حذف نمایید:
</h3>

<pre align="left">
<code dir="ltr">
rm -rf node_modules package-lock.json
</code>
</pre>

<h3>
▶️ سپس دستور زیر را با نسخه‌ی جدید Node اجرا نمایید:
</h3>

<pre align="left">
<code dir="ltr">npm install</code>
</pre>

<h4>
❗ ۳. در نهایت، برای اجرای Storybook، دستور زیر را وارد کنید:
</h4>

<pre align="left">
<code dir="ltr">npm run storybook</code>
</pre>
