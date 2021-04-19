# aws-url-signer
This Dart library **signs Amazon Web Services (AWS) URLs** with the given credentials in contrast to signing the header entries. This is particularly helpful to connect to **Amazon WebSocket API Gateway secured with IAM authorizer**.

I created this work mainly because *Amazon Amplify* does not provide any easy mechanism to sign the URLs to be able to connect to secured WebSocket endpoints, unfortunately. I spent over a week between searching and reading the source codes of different projects to be able to connect my Flutter App to my AWS secured WebSocket API Gateway backend.

Now, after I got this working, I am glad to share this work, maybe it can save someone's day.
