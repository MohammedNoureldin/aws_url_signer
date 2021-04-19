# aws_url_signer

This Dart library **signs Amazon Web Services (AWS) URLs** with the given credentials in contrast to signing the header entries. This is particularly helpful to connect to **Amazon WebSocket API Gateway secured with IAM authorizer**.

I created this work mainly because *Amazon Amplify* does not provide any easy mechanism to sign the URLs to be able to connect to secured WebSocket endpoints, unfortunately. I spent over a week between searching and reading the source codes of different projects to be able to connect my Flutter App to my AWS secured WebSocket API Gateway backend.

Now, after I got this working, I am glad to share this work, maybe it can save someone's day.

**Pull Requests are welcome.**

### Credits further readings

Many thanks to [Ivan Djuricic](https://github.com/ivandjuricic), because this code is inspired by a [signing code](https://gist.github.com/ivandjuricic/eac871ad2a68fa7775baf2497252fef3) written by him in Python.

Skimming the [this code file](https://github.com/agilord/aws_client/blob/master/aws_client/lib/src/request.dart) also helped me to replace some critical python parts with their Dart equivalents.

A look on the official documentation [Signing AWS Requests V4](https://docs.aws.amazon.com/general/latest/gr/sigv4_signing.html) from Amazon will make the code makes much more sense.
