# Qt Code Editor Widget
It's widget for editing/viewing code.

(It's not project from Qt example)

## Requirements
0. C++11 featured compiler.
0. Qt 5.

## Abilities
1. Auto parentheses.
1. Different highlight rules.
1. Auto indentation.
1. Replace tabs with spaces.
1. GLSL Completion rules.
1. GLSL highlight rules.
1. C++ highlight rules.
1. Qt Creator styles.

## Build
It's CMake based library so it can be used as submodule. (See example)
But here is the steps to build it as static library (for external use for example).

1. Clone repo: `git clone https://github.com/Megaxela/QCodeEditor`
1. Go into repo: `cd QCodeEditor`
1. Create build folder: `mkdir build`
1. Go into build folder: `cd build`
1. Generate build file for your compiler: `cmake ..`
    1. If you need to build example, specify `-DBUILD_EXAMPLE=On` on this step.
1. Build library: `cmake --build .`

## Example

By default `QCodeEditor` uses standard QtCreator theme. But you may specify
you own by parsing it with `QSyntaxStyle`. Example uses [Dracula](https://draculatheme.com) theme.
(See example for more) 

<img src="https://github.com/Megaxela/QCodeEditor/blob/master/example/image/preview.png">

## LICENSE

<img align="right" src="http://opensource.org/trademarks/opensource/OSI-Approved-License-100x137.png">

Library is licensed under the [MIT License](https://opensource.org/licenses/MIT)

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