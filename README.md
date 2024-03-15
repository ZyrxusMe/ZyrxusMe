```cpp
#include <iostream>
#include <map>
#include <string>

std::map<std::string, std::string> wizly(const std::string& lang) {
    std::map<std::string, std::string> response;

    if (lang.empty()) {
        response["msg"] = "Please specify a language.";
    } else if (lang == "en") {
        response = {{"code", "200"}, {"title", "Weasley"}, {"desc", "He's a maniac who messes with the code like crazy"}};
    } else if (lang == "tr") {
        response = {{"code", "200"}, {"title", "Weasley"}, {"desc", "Kodlarla deli gibi uğraşan bir manyak"}};
    } else {
        response["msg"] = "Please specify a correct language";
    }

    return response;
}

int main() {
    std::string lang;
    std::cout << "Enter language (en or tr): ";
    std::cin >> lang;

    std::map<std::string, std::string> result = wizly(lang);

    for (const auto& pair : result) {
        std::cout << pair.first << ": " << pair.second << std::endl;
    }

    return 0;
}
```

<html>
<br><br>
    <p align="center">
    <img src="https://github-profile-trophy.vercel.app/?username=ZyrxusMe&theme=onedark">
    <br><br>
    <img src="https://github-readme-stats.vercel.app/api?username=ZyrxusMe&theme=dark">
</p>
</html>
