# rtos-m0-3
The FreeRTOS 202212.00 release updates FreeRTOS Kernel, FreeRTOS+TCP, coreMQTT, corePKCS11, coreHTTP, coreJSON, AWS IoT Over-the-air-Updates (OTA), AWS IoT Device Shadow, AWS IoT Jobs, AWS IoT Device Defender, Backoff Algorithm, AWS IoT Fleet Provisioning, coreSNTP, SigV4, and FreeRTOS Cellular Interface libraries to their LTS 2.0 versions. It also updates coreMQTT Agent to v1.2.0 to be compatible with coreMQTT v2.X.X, and updates MbedTLS to v3.2.1. This release also adds Visual Studio static library projects for the FreeRTOS Kernel, FreeRTOS+TCP, Logging, MbedTLS, coreHTTP, and corePKCS11. With the addition of the static library projects, all Visual Studio projects have been updated to use them. Additionally, all demos dependent on coreMQTT have been updated to work with coreMQTT v2.X.X.

Getting started
The FreeRTOS.org website contains a FreeRTOS Kernel Quick Start Guide, a list of supported devices and compilers, the API reference, and many other resources.

Getting help
You can use your Github login to get support from both the FreeRTOS community and directly from the primary FreeRTOS developers on our active support forum. The FAQ provides another support resource.

Cloning this repository
This repo uses Git Submodules to bring in dependent components.

Note: If you download the ZIP file provided by the GitHub UI, you will not get the contents of the submodules. (The ZIP file is also not a valid git repository)

If using Windows, because this repository and its submodules contain symbolic links, set core.symlinks to true with the following command:

git config --global core.symlinks true
In addition to this, either enable Developer Mode or, whenever using a git command that writes to the system (e.g. git pull, git clone, and git submodule update --init --recursive), use a console elevated as administrator so that git can properly create symbolic links for this repository. Otherwise, symbolic links will be written as normal files with the symbolic links' paths in them as text. This gives more explanation.

To clone using HTTPS:

git clone https://github.com/FreeRTOS/FreeRTOS.git --recurse-submodules
