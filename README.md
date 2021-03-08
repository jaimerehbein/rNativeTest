code in reactnative 0.63

obs:
The result is following error.

** BUILD FAILED **

The following build commands failed:
CompileC /Users/LeeMoonki/Desktop/FirstNative/ios/build/FirstNative/Build/Intermediates.noindex/Pods.build/Debug-iphonesimulator/Folly.build/Objects-normal/x86_64/Unicode.o /Users/LeeMoonki/Desktop/TestNativeProject/ios/Pods/Folly/folly/Unicode.cpp normal x86_64 c++ com.apple.compilers.llvm.clang.1_0.compiler
(1 failure)

To see the exact error, I run the workspace of this project in the Xcode(v10.3) then the following error is occurred.


Error found when deploying ios emulator, could be solved by changing the following line of code:

replace use_flipper! with use_flipper!({ 'Flipper-Folly' => '2.3.0' }) in your Podfile, then remove Podfile.lock and run pod install



# rNativeTest
