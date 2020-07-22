# Dialogflow SDK generated from proto files for Android


This is repository showing straggles with creating client for dialogflow on Android from proto files

# Copy and paste proto files

* Setup protoc gradle plugin according to example https://github.com/grpc/grpc-java/blob/v1.30.1/examples/android/helloworld/app/build.gradle
* Fix duration.proto problem https://github.com/protocolbuffers/protobuf/pull/7738 and see https://github.com/rudovjan/dialogflow-proto-android/blob/e885005505eaa91eb21828fc0d4b73bbf7ffd38a/app/build.gradle#L48)
* Fix annotation problem in operations.proto (https://github.com/rudovjan/dialogflow-proto-android/blob/e885005505eaa91eb21828fc0d4b73bbf7ffd38a/app/src/main/proto/google/longrunning/operations.proto#L34)
* Copy and paste missing client files and stub (see https://github.com/rudovjan/dialogflow-proto-android/blob/master/app/src/main/java/com/google/cloud/dialogflow/v2beta1)
* Fix client files (https://github.com/rudovjan/dialogflow-proto-android/blob/master/app/src/main/java/com/google/cloud/dialogflow/v2beta1/stub/GrpcSessionsStub.java --> see Rudovsky note)
* Exclude stuff ... so collisions are avoided (https://github.com/rudovjan/dialogflow-proto-android/blob/master/app/build.gradle --> see Rudovsky note)


