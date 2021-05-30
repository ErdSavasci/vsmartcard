# Virtual Smart Card Architecture

Virtual Smart Card Architecture is an umbrella project for various
projects concerned with the emulation of different types of smart card readers
or smart cards themselves.

Currently the following projects are part of Virtual Smart Card Architecture: 

- [Virtual Smart Card](http://frankmorgner.github.io/vsmartcard/virtualsmartcard/README.html)
- [Remote Smart Card Reader](http://frankmorgner.github.io/vsmartcard/remote-reader/README.html)
- [Android Smart Card Emulator](http://frankmorgner.github.io/vsmartcard/ACardEmulator/README.html)
- [PC/SC Relay](http://frankmorgner.github.io/vsmartcard/pcsc-relay/README.html)
- [USB CCID Emulator](http://frankmorgner.github.io/vsmartcard/ccid/README.html)

Please refer to [our project's website](http://frankmorgner.github.io/vsmartcard) for more information.

[![Travis CI Build Status Image](https://img.shields.io/travis/frankmorgner/vsmartcard/master.svg?label=Travis%20CI%20build)](https://travis-ci.org/frankmorgner/vsmartcard) [![AppVeyor CI Build Status Image](https://img.shields.io/appveyor/ci/frankmorgner/vsmartcard/master.svg?label=AppVeyor%20build)](https://ci.appveyor.com/project/frankmorgner/vsmartcard) [![Coverity Scan Status](https://img.shields.io/coverity/scan/3987.svg?label=Coverity%20scan)](https://scan.coverity.com/projects/3987)

### Update: 2021/05/31

#### Steps to build and install on Windows 
Note: These steps are valid for Visual Studio 2019. Some other further steps may be needed for other VS versions.
<br>
1. Run git submodule update --init --recursive when cloned the repository.
2. Install Wix Toolset build tools from https://wixtoolset.org/releases/
3. Install Wix Extension for Visual Studio
4. Determine the correct solution platform and solution configuration (x86/x64)
5. Build the solution (Consists of 3 projects)
6. Create 'BixVReader.ini' file in C:\Windows
7. Install via BixVReaderInstaller.msi
8. Add the generated 'BixVReader.cer' certificate to the Trusted Root Certification Authorities and Trusted Publishers certificate stores for Local Machine via 'certlm.msc'.
9. Update the driver with the driver package files from Device Manager.
10. Voila! 'Bix Virtual Smart Card Reader' should be seen on Device Manager.

<br>
<br>
<br>




