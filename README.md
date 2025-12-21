<div align="center">

# 🛡️ uBlock CustomFilters

### Advanced filter lists for enhanced web browsing

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![uBlock Origin](https://img.shields.io/badge/uBlock%20Origin-Compatible-red.svg)](https://github.com/gorhill/uBlock)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/Suurp/uBlock-CustomFilters/graphs/commit-activity)
[![Stars](https://img.shields.io/github/stars/Suurp/uBlock-CustomFilters?style=social)](https://github.com/Suurp/uBlock-CustomFilters/stargazers)

[📥 Quick Install](#-quick-installation) • [📖 Documentation](#-features) • [🤝 Contributing](#-contributing) • [❓ FAQ](#-faq)

---

</div>

## 📋 Overview

**uBlock CustomFilters** is a curated collection of advanced filter lists designed for **uBlock Origin**, featuring two specialized filter sets:

<table>
<tr>
<td width="50%" valign="top">

### 🔗 LinkGuard Filter
Bypass shortlinks automatically with timer acceleration, ad removal, anti-adblock evasion, and automated navigation.

**Popular services:** link-to.net, exe.io, ouo.io, shrinkme.io, linkvertise

</td>
<td width="50%" valign="top">

### 💰 CryptoBlock Filter
Optimize crypto faucets and PTC sites with claim automation, timer boost, captcha handling, and iframe removal.

**Popular platforms:** FaucetPay, auto-faucets, ClixSense, NeoBux

</td>
</tr>
</table>

> [!WARNING]
> These filters use advanced web manipulation techniques (timer optimization, automated interactions, script modifications). Intended for educational and research purposes. Review website Terms of Service before use.

---

## 🚀 Quick Installation

### Method 1: One-Click Subscribe (Recommended)

Click the subscribe button for your desired filter list:

| Filter List | Purpose | Subscribe |
|------------|---------|-----------|
| **🔗 LinkGuard** | Shortlink bypass, ad removal, timer boost | [![Subscribe](https://img.shields.io/badge/Subscribe-LinkGuard-blue?style=for-the-badge)](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/Suurp/uBlock-CustomFilters/refs/heads/main/filters-shortlinks.txt&title=LinkGuard%20-%20Shortlinks%20Bypass) |
| **💰 CryptoBlock** | Faucet optimization, PTC boost, auto-claim | [![Subscribe](https://img.shields.io/badge/Subscribe-CryptoBlock-green?style=for-the-badge)](https://subscribe.adblockplus.org/?location=https://raw.githubusercontent.com/Suurp/uBlock-CustomFilters/refs/heads/main/filters-faucets.txt&title=CryptoBlock%20-%20Faucets%20Optimizer) |

### Method 2: Manual Import

1. Open **uBlock Origin** dashboard
2. Navigate to **"Filter lists"** tab
3. Scroll to **"Custom"** section
4. Check **"Import..."** and paste the URL:

```
LinkGuard:    https://raw.githubusercontent.com/Suurp/uBlock-CustomFilters/refs/heads/main/filters-shortlinks.txt
CryptoBlock:  https://raw.githubusercontent.com/Suurp/uBlock-CustomFilters/refs/heads/main/filters-faucets.txt
```

5. Click **"Apply changes"**

---

## ⚙️ Required Configuration

> [!IMPORTANT]
> Trust configuration is mandatory for filters to work correctly.

These filters use advanced techniques requiring explicit trust configuration:

1. Open **uBlock Origin dashboard** → **Settings**
2. Enable **"I am an advanced user"** (⚙️ icon appears)
3. Click the **⚙️ gear icon**
4. Locate **`trustedListPrefixes`**
5. Add to existing value (space-separated):
   ```
   https://raw.githubusercontent.com/Suurp/uBlock-CustomFilters/
   ```

> [!TIP]
> **Example configuration:**
> ```
> Before:  ublock-
> After:   ublock- https://raw.githubusercontent.com/Suurp/uBlock-CustomFilters/
> ```

6. Click **"Apply changes"** and restart browser

---

## ✨ Features & Technical Details

<details>
<summary><b>🔧 How it works</b></summary>

**Core Techniques:**
- Scriptlet injection for behavior modification
- Timer manipulation and acceleration
- DOM element removal and modification
- Event listener interception
- Automated form interactions
- Client-side captcha bypass (when improperly validated)

**Compatible with:** All browsers supporting uBlock Origin (Chrome, Firefox, Edge, Opera, Brave)
</details>

---

## 🛠️ Advanced Usage

### Testing & Verification

After installation:

1. **Visit a test site** (e.g., link-to.net, exe.io)
2. **Open uBlock Logger** (dashboard → Logger icon)
3. **Observe filter activity** in real-time
4. **Verify bypass functionality** works as expected

### Troubleshooting

> [!NOTE]
> Some sites use server-side validation that cannot be bypassed client-side.

<details>
<summary><b>Bypass not working?</b></summary>

**Checklist:**
- ✅ Verify `trustedListPrefixes` is configured correctly
- ✅ Clear browser cache and cookies
- ✅ Check uBlock Origin logger for errors
- ✅ Temporarily disable other extensions
- ✅ Ensure filters are up-to-date
- ✅ Report persistent issues on GitHub

**Common Issues:**
- **Site still shows timer**: Server-side validation in use
- **Captcha not bypassed**: Only client-side captchas work
- **Page broken**: Possible conflict with other filters

</details>

### Best Practices

> [!CAUTION]
> **Recommended:** Use only with uBlock Origin's default filters. Adding third-party lists may cause conflicts or errors.

> [!TIP]
> - Keep filters updated regularly
> - Test on a few sites before widespread use
> - Report issues on GitHub for quick fixes
> - Consider supporting sites you use frequently

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### 🐛 Report Issues

> [!NOTE]
> When reporting issues, please include:
> - Site URL and specific problem
> - Browser console errors (F12 → Console)
> - uBlock Origin logger output
> - Which filter list (LinkGuard/CryptoBlock)

Open an issue for:
- Sites not bypassing correctly
- Broken functionality after update
- New site support requests
- Filter conflicts or errors

### 💡 Submit Filters

> [!IMPORTANT]
> All contributions must be tested thoroughly and follow ethical guidelines.

**To contribute new filters:**

1. **Fork** this repository
2. **Test** your filters on latest uBlock Origin
3. **Document** the bypass technique used
4. **Submit** a Pull Request with clear description

### 📚 Improve Documentation

Help improve this README by:
- Fixing typos or unclear sections
- Adding examples or use cases
- Translating to other languages
- Creating tutorials or guides

---

## ❓ FAQ

<details>
<summary><b>Are these filters legal to use?</b></summary>

These filters use techniques similar to popular browser extensions and userscripts. Legality depends on usage:
- ✅ Personal learning and research: Generally acceptable
- ✅ Understanding web technologies: Completely fine
- ⚠️ Website ToS compliance: User's responsibility to review
- ❌ Large-scale abuse: Against site policies and not recommended

**Bottom line:** Use responsibly, respect policies, and you'll be fine. These are educational tools.
</details>

<details>
<summary><b>Will these filters speed up timers?</b></summary>

Yes, many timers can be accelerated or bypassed. However:
- Effectiveness varies by site implementation
- Server-side validated timers cannot be bypassed
- Some sites detect and block timer manipulation
- Results depend on bypass method available
</details>

<details>
<summary><b>Do I need both filter lists?</b></summary>

No, choose based on your needs:
- **LinkGuard only**: For shortlink services
- **CryptoBlock only**: For crypto faucets and PTC sites
- **Both**: If you use both types of services

Lists are independent and can be used separately.
</details>

<details>
<summary><b>Why trust configuration required?</b></summary>

Advanced techniques (scriptlet injection, timer manipulation) require explicit trust for security. This is a uBlock Origin safety feature preventing arbitrary code execution.
</details>

<details>
<summary><b>Do these work on mobile?</b></summary>

Yes, but only on:
- ✅ Firefox for Android (with uBlock Origin)
- ✅ Kiwi Browser (with Chrome extensions)
- ❌ Chrome mobile (no extension support)
- ❌ Safari mobile (limited extension support)
</details>

<details>
<summary><b>How to update filters manually?</b></summary>

1. Open uBlock Origin dashboard
2. Go to "Filter lists" tab
3. Click the clock icon 🕐 (Update now)
4. Wait for update to complete
</details>

<details>
<summary><b>Can I contribute my own bypass filters?</b></summary>

Absolutely! We welcome contributions:
1. Test filters thoroughly
2. Document the technique
3. Ensure ethical use
4. Submit detailed Pull Request

See [Contributing](#-contributing) section for details.
</details>

---

## 🔗 Related Resources

- 📚 [uBlock Origin Wiki](https://github.com/gorhill/uBlock/wiki)
- 🛡️ [uBlock Resources Library](https://github.com/gorhill/uBlock/wiki/Resources-Library)
- 📖 [Scriptlet Documentation](https://github.com/gorhill/uBlock/wiki/Static-filter-syntax#scriptlet-injection)
- 💬 [r/uBlockOrigin Community](https://www.reddit.com/r/uBlockOrigin/)
- 🔧 [Filter Syntax Guide](https://github.com/gorhill/uBlock/wiki/Static-filter-syntax)

---

## 📜 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

**In simple terms:** Free to use, modify, and share. Provided as-is for educational purposes. Use responsibly.

---

## 🙏 Acknowledgments

- **uBlock Origin Team** - For the incredible ad blocker
- **Community Contributors** - For testing and feedback
- **Filter List Maintainers** - For inspiration and techniques

---

## 📞 Support

**Need help?**

- 📧 [Open an Issue](https://github.com/Suurp/uBlock-CustomFilters/issues/new)
- ⭐ Star this repository if you find it useful!

---

<div align="center">

**Made with ❤️ for optimized browsing**

[⬆ Back to Top](#-ublock-customfilters)

---

[![GitHub stars](https://img.shields.io/github/stars/Suurp/uBlock-CustomFilters?style=social)](https://github.com/Suurp/uBlock-CustomFilters/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/Suurp/uBlock-CustomFilters?style=social)](https://github.com/Suurp/uBlock-CustomFilters/forks)
[![GitHub watchers](https://img.shields.io/github/watchers/Suurp/uBlock-CustomFilters?style=social)](https://github.com/Suurp/uBlock-CustomFilters/watchers)

</div>
