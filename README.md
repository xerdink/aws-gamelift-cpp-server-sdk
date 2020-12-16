# AWS GameLift C++ Server SDK

## What is it?
This is a working and buildable version of [GameLift](https://aws.amazon.com/tr/gamelift/) C++ server SDK.  
I know that AWS SDK can be downloaded from their [link](https://gamelift-release.s3-us-west-2.amazonaws.com/GameLift_11_11_2020.zip) but, 
the main problems are:
* SDK is dependent on Protobuf v3.3.0 because AWS chose not to publish `.proto` files. They have embedded compiled `.pb.cc` and header.
* It also has dependency on [socket.io-client-cpp](https://github.com/socketio/socket.io-client-cpp) which is outdated.

## Solution :fire:
This repo has `.proto` file and you can generate compiled C++ output on any version you want.

## Building
* I have used Visual Studio 2019 C++ build tools v142 and with [vcpkg](https://github.com/microsoft/vcpkg) installed Boost
and Protobuf v3.14.0.
