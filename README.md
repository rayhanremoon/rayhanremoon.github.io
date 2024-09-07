# rayhanremoon.github.io/your_php_script.html

<!DOCTYPE html>
<script>
    window.onload = function () {
        TruecallerSDK.init({
            clientId: "7dB6bab5f95bd24014da2a373d87bc6f397f0",
            callbackUrl: "rayhanremoon.github.io/your_php_script.php", // Your PHP script URL
            redirect: true,
            mobileOnly: true
        });

        TruecallerSDK.login(document.getElementById("truecaller-login"), function (response) {
            // Send the response data to your server
            fetch('rayhanremoon.github.io/your_php_script.php', {
                method: 'POST',
                headers: {
                    'Content-Type': 'application/json'
                },
                body: JSON.stringify(response)
            })
            .then(response => response.json())
            .then(data => {
                console.log(data); // Handle server response
            });
        });
    };
</script>
TruecallerSDK.login(document.getElementById("truecaller-login"), function (response) {
                // Success response handling
                console.log(response);  // এখানে আপনি response দেখে ডেটা প্রসেস করতে পারবেন
            });
        };
    </script>
</body>
</html>
