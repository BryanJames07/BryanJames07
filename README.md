- 👋 Hi, I’m @BryanJames07
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
BryanJames07/BryanJames07 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
def PalindromeCheck(s):
    s = s.lower()
    length = len(s)
    if length < 2:
        return True
    elif s[0] == s[length - 1]:
        return PalindromeCheck(s[1: length - 1])

    else:
        return False


userIn = input("Input a Word or number/s: ")
ans = PalindromeCheck(userIn)

if ans:
    print(userIn + " is a Palindrome")

else:
    print(userIn + " is not a Palindrome")
