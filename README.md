# botright-driver-autoinstall
This was made to automatically install playwright drivers by using the playwright-driver-autoinstall module by me alongside botright.

## Install

```bash
pip install git+https://github.com/BlueSchnabeltier/botright-driver-autoinstall.git
```

---

## Usage

### Botright is only available in async mode.
### It is fully plugable with your existing playwright code. You only have to change your browser initialization!

```py
import asyncio

import botright


async def main():
    botright_client = await botright.Botright(headless=False)
    browser = await botright_client.new_browser()
    page = await browser.new_page()

    # Continue by using the Page

    await botright_client.close()

if __name__ == "__main__":
    asyncio.run(main())
```

Read the [Documentation](https://botright.readthedocs.io/en/latest)

---

## Captcha Solving

Botright is able to solve a wide viarity of Captchas.
For Documentation of these functions visit [BotrightDocumentation](botright.md).

It uses Computer Vision/Artificial Intelligence and other Methods to solve these Captchas.

You dont need to pay for any Captcha Solving APIs and you can solve Captchas with just one simple function call.

Here all Captchas supported as of now:

| Captcha Type | Supported | Success Rate |
|:--------------:|:--------------:|--------------|
| `hCaptcha` | ✔️ | 50%-90% (Depending on topicality of new Types) |
| `reCaptcha` | ✔️ | 30%-50% |
| `geeTestv3` |
| v3 Intelligent Mode | ✔️ | 100% |
| v3 Slider Captcha | ✔️ | 100% |
| v3 Nine Captcha | ✔️ | 50% |
| v3 Icon Captcha | ✔️ | 70% |
| v3 Space Captcha | ❌ | 0% |
| `geeTestv4` |
| v4 Intelligent Mode | ✔️ | 100% |
| v4 Slider Captcha | ✔️ | 100% |
| v4 GoBang Captcha | ✔️ | 100% |
| v4 Icon Captcha | ✔️ | 60% |
| v4 IconCrush Captcha | ✔️ | 100% |

## Development

Read the [CONTRIBUTING.md](https://github.com/Vinyzu/Botright/blob/main/CONTRIBUTING.md) file.

---

## Copyright and License
© [Vinyzu](https://github.com/Vinyzu/)

[GNU GPL](https://choosealicense.com/licenses/gpl-3.0/)

(Commercial Usage is allowed, but source, license and copyright has to made available. Botright does not provide and Liability or Warranty)

---

## Thanks to

[QIN2DIM](https://github.com/QIN2DIM/) (For his great AI work) (Note his GitHub got banned)

[MaxAndolini](https://github.com/MaxAndolini) (For shared knowledge of hCaptcha bypassing)

[CreativeProxies](https://creativeproxies.com) (For sponsoring me with Proxies)

---

![Version](https://img.shields.io/badge/Botright-v0.2.2-blue)
![License](https://img.shields.io/badge/License-GNU%20GPL-green)
![Python](https://img.shields.io/badge/Python-v3.x-lightgrey)

[![my-discord](https://img.shields.io/badge/My_Discord-000?style=for-the-badge&logo=google-chat&logoColor=blue)](https://discordapp.com/users/935224495126487150)
[![buy-me-a-coffee](https://img.shields.io/badge/Buy_Me_A_Coffee-000?style=for-the-badge&logo=ko-fi&logoColor=brown)](https://ko-fi.com/vinyzu)
