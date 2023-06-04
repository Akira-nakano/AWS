# AWS

lambda-consoleloginは、特定のユーザーグループがサインインした時のみSNS通知し、メトリクスにカウントさせる場合のLambda関数。
必要となるIAMロールは、Consolelogin-roleを参照すること。
また、サブスクリプションフィルターに設定するフィルターは、{ $.eventType = "AwsConsoleSignIn" }
