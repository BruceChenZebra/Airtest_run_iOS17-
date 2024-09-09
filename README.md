# Airtest_run_iOS17+
how to run iOS 17 + by using Airtest

## Precondition
### Windows
1. you need to build the WebDriverAgent ipa by Mac (https://github.com/facebookarchive/WebDriverAgent)
2. you need to install the latest go-ios tool in URL https://github.com/danielpaulus/go-ios/releases, and add environment variables
3. you need to download the latest wintun.dll in URL https://www.wintun.net/, and put it in the path: C:/Windows/system32
4. run the command `ios tunnel start` with administrator privileges

### iOS
1. use Xcode to build WebDriverAgent into your phone (https://github.com/facebookarchive/WebDriverAgent)
2. run command: `npm install -g go-ios`
3. run command: `sudo ios tunnel start`

## update the your variable parameters below in ios_17_18_demo.py
1. WDA_Package_Name = 'com.xxxxx.WebDriverAgentRunner.xctrunner' 
2. uuid = "0000XXXX-000451212381231A"
3. WDA_ipa_path = r'tidevice install WebDriverAgent.ipa'