# rayhanremoon.github.io

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Truecaller Verification</title>
    <!-- Truecaller SDK Script -->
    <script
        type="text/javascript"
        src="https://sdk.truecaller.com/v2.0/truecaller-sdk.js"
        async
    ></script>
</head>
<body>
    <h2>Truecaller Verification</h2>
    <!-- Button to trigger Truecaller login -->
    <div id="truecaller-login"></div>

    <script>
        window.onload = function () {
            // Truecaller SDK initialization
            TruecallerSDK.init({
                clientId: "IiO2U050e07a511c942999a1efd1c6c2f0dc8", // আপনার ক্লায়েন্ট আইডি
                callbackUrl: "https://rayhanremoon.github.io", // আপনার Callback URL
                redirect: true,
                mobileOnly: true
            });

            // Trigger Truecaller login
            TruecallerSDK.login(document.getElementById("truecaller-login"), function (response) {
                // Success response handling
                console.log(response);  // এখানে আপনি response দেখে ডেটা প্রসেস করতে পারবেন
            });
        };
    </script>
</body>
</html>
