![代码质量](https://img.shields.io/badge/Code_Quality-Spaghetti-red)
![Bug 数量](https://img.shields.io/badge/Bugs_Found-Too_Many_To_Count-orange)
![维护者](https://img.shields.io/badge/Maintained_By-Coffee_and_Tears-blue)
</p>

`Surge5` `Firewall` `linux`
> *Talk is cheap. Show me the code.* — Linus Torvalds  


---

## 📦 仓库结构
（假设结构，视实际改动）


`⚠️注意事项`
* 本配置为个人自用
* 作者不对使用本配置可能导致的任何问题负责

![版本](https://img.shields.io/badge/version-1.0.0-blue)
![许可证](https://img.shields.io/badge/license-MIT-green)

<!DOCTYPE html>
<html lang="zh-Hans">
<head>
    <meta charset="UTF-8">
    <title>基本資料表單</title>
    <script>
      function handleSubmit(event) {
        event.preventDefault();
        alert("您的資料已成功送出！");
      }
    </script>
</head>
<body>
    <form onsubmit="handleSubmit(event)">
        <label for="name">姓名：</label>
        <input type="text" id="name" name="name" required><br><br>
        
        <label for="email">Email：</label>
        <input type="email" id="email" name="email" required><br><br>
        
        <label for="phone">電話號碼：</label>
        <input type="tel" id="phone" name="phone" required><br><br>
        
        <button type="submit">送出</button>
    </form>
</body>
</html>


