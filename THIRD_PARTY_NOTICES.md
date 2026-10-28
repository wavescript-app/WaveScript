# WaveScript – Third-Party Notices

WaveScript itself is licensed under the terms in `LICENSE.md`. It
includes or depends on the following third-party components, each of
which remains under its own licence. These terms apply to those
components only, not to WaveScript.

| Component | Used for | Licence |
|---|---|---|
| [PySide6 / Qt for Python](https://www.qt.io/qt-for-python) (Qt 6) | User interface, audio capture | LGPL v3 (and GPL / commercial) |
| [faster-whisper](https://github.com/SYSTRAN/faster-whisper) | On-device speech-to-text | MIT |
| [CTranslate2](https://github.com/OpenNMT/CTranslate2) | Inference engine for faster-whisper | MIT |
| [OpenAI Whisper](https://github.com/openai/whisper) models (`small.en`, converted to CTranslate2 format by [Systran](https://huggingface.co/Systran)) | Speech recognition model weights | MIT |
| [NumPy](https://numpy.org) | Audio array handling | BSD 3-Clause |
| [Pillow](https://python-pillow.org) | Image handling | MIT-CMU (HPND) |
| [pyspellchecker](https://github.com/barrust/pyspellchecker) | Offline spell checking and its English word list | MIT |
| [comtypes](https://github.com/enthought/comtypes) (Windows only) | Microphone mute fix | MIT |
| [Python](https://www.python.org) runtime | Application runtime | PSF License |
| [PyInstaller](https://pyinstaller.org) (build tool) | Packaging the app | GPL v2 with bootloader exception (output is not GPL-restricted) |

## Qt / PySide6 (LGPL v3)

WaveScript uses PySide6 and Qt as dynamically linked libraries, which
are included unmodified in the packaged application. Under the LGPL
you may replace them with your own build of the same libraries. The
LGPL v3 text is at <https://www.gnu.org/licenses/lgpl-3.0.html> and
Qt's source code is available from <https://www.qt.io/download-open-source>
and <https://code.qt.io>.

## MIT-licensed components

faster-whisper, CTranslate2, the Whisper models, pyspellchecker and
comtypes are each distributed under the MIT licence:

> Permission is hereby granted, free of charge, to any person obtaining
> a copy of this software and associated documentation files (the
> "Software"), to deal in the Software without restriction, including
> without limitation the rights to use, copy, modify, merge, publish,
> distribute, sublicense, and/or sell copies of the Software, and to
> permit persons to whom the Software is furnished to do so, subject to
> the following conditions:
>
> The above copyright notice and this permission notice shall be
> included in all copies or substantial portions of the Software.
>
> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
> EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
> MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
> IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
> CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
> TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
> SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Copyright holders:

- faster-whisper: Copyright (c) 2023 SYSTRAN
- CTranslate2: Copyright (c) OpenNMT contributors
- Whisper: Copyright (c) 2022 OpenAI
- pyspellchecker: Copyright (c) 2016 Tyler Barrus
- comtypes: Copyright (c) Thomas Heller, Enthought and contributors

## Other components

NumPy (BSD 3-Clause), Pillow (MIT-CMU/HPND) and Python (PSF) are
distributed under their own permissive licences. Their full texts ship
with the respective packages and are available from the project
websites listed above.

---

*Licence details were compiled from each project's published terms.
Please check the versions pinned in `requirements.txt` against the
projects' current licence files before redistribution.*
