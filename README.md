# Release Api Spam SMS

### ĐỂ SỬ DỤNG API BẰNG CÁCH CALLBACK BẰNG CODE BÊN DƯỚI

### PHP:
```php
header('Content-Type: application/json');
$ch = curl_init("https://your-domain.com/spam-sms.php?sdt=phone"); // phone là số điện thoại cần điền
curl_setopt_array($ch, [
    CURLOPT_HTTPHEADER => ["X-WusTeam: 2bac6acbcd29-020f-4cee-ae0d-7ad267d1aa86"],
    CURLOPT_RETURNTRANSFER => true
]);
echo curl_exec($ch);
curl_close($ch);
```
### CURL

```cmd
curl -H "X-WusTeam: xxx" https://your-domain.com/spam-sms.php?sdt=phone
```
