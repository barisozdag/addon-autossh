# barisozdag's Personal Home Assistant Add-ons: Autossh

[![GitHub Release][releases-shield]][releases]
![Project Stage][project-stage-shield]
[![License][license-shield]](LICENSE.md)

![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]
![Supports armhf Architecture][armhf-shield]
![Supports armv7 Architecture][armv7-shield]
![Supports i386 Architecture][i386-shield]

[![Github Actions][github-actions-shield]][github-actions]
![Project Maintenance][maintenance-shield]
[![GitHub Activity][commits-shield]][commits]

Simple autossh addon. The addon creates a ssh keypair, and uses it to
connect to to the given host. The public key can be found in the log after
the first startup.

[:books: Read the full add-on documentation][docs]

## About

Simple autossh addon. The addon creates a ssh keypair, and uses it
to connect to to the given host. The public key can be found in the
log after the first startup.

Remember to set `GatewayPorts clientspecified` in sshd-config if you
would like to open ports on other interfaces than localhost.

**IMPORTANT**: If you set `GatewayPorts yes`, all forwarded ports will
listen on all interfaces, `0.0.0.0`. `GatewayPorts clientspecified`
is preferable.

## Support

Got questions?

You could [open an issue here][issue] GitHub.

## Contributing

This is an active open-source project. I'm always open to people who want to
use the code or contribute to it.

Thank you for being involved! :heart_eyes:

## Authors & contributors

The original setup of this repository is by [Odin Udegal][odinuge].
This repository is a copy of [Odin Ugedal's Hassio Addons][odin_hassio_addons]
without the `frpc` addon.

For a full list of all authors and contributors,
check [the contributor's page][contributors].

## License

MIT License

Copyright (c) 2017-2020 Odin Ugedal

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[armhf-shield]: https://img.shields.io/badge/armhf-yes-green.svg
[armv7-shield]: https://img.shields.io/badge/armv7-yes-green.svg
[i386-shield]: https://img.shields.io/badge/i386-yes-green.svg
[commits-shield]: https://img.shields.io/github/commit-activity/y/barisozdag/addon-autossh.svg
[commits]: https://github.com/barisozdag/addon-autossh/commits/main
[contributors]: https://github.com/barisozdag/addon-autossh/graphs/contributors
[docs]: https://github.com/barisozdag/addon-autossh/blob/main/autossh/DOCS.md
[odinuge]: https://github.com/odinuge
[odin_hassio_addons]: https://github.com/odinuge/hassio-addons
[github-actions-shield]: https://github.com/barisozdag/addon-autossh/workflows/CI/badge.svg
[github-actions]: https://github.com/barisozdag/addon-autossh/actions
[issue]: https://github.com/barisozdag/addon-autossh/issues
[license-shield]: https://img.shields.io/github/license/barisozdag/addon-autossh.svg
[maintenance-shield]: https://img.shields.io/maintenance/yes/2023.svg
[project-stage-shield]: https://img.shields.io/badge/project%20stage-production%20ready-brightgreen.svg
[releases-shield]: https://img.shields.io/github/release/barisozdag/addon-autossh.svg
[releases]: https://github.com/barisozdag/addon-autossh/releases
[repository]: https://github.com/barisozdag/haddons-repo
