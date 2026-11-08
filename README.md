# PassGuard — Python CLI Password Strength Analyzer & Generator

**PassGuard** is an interactive command-line utility written in Python that evaluates password complexity and generates customizable passwords based on user-selected character classes.

---

## Features

- **Password Complexity Scoring (`sifre_guclulugu`):** Evaluates candidate passwords on a `0/4` to `4/4` scale across four character categories (lowercase letters, uppercase letters, digits, and punctuation symbols).
- **Customizable Password Generation (`guclu_sifre_uret`):** Interactive CLI prompts allow users to toggle lowercase, uppercase, numeric, and special character sets and specify custom output lengths (defaulting to 12 characters on invalid input).
- **Zero Persistence / No Logging:** All evaluations and generated passwords occur strictly in memory via standard input/output (`stdin`/`stdout`) and are never written to disk or log files.

---

## Tech Stack & Requirements

- **Language:** Python 3.8+
- **Dependencies:** Python Standard Library only (`random`, `string`)

---

## Project Structure

```text
PassGuard/
├── main.py         # CLI entry point, strength evaluator, and password generator
├── .gitignore      # Python gitignore configuration
└── README.md       # Project documentation
```

---

## Installation & Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mert-carli/PassGuard.git
   cd PassGuard
   ```

2. **Run the application:**
   ```bash
   python main.py
   ```

### Example CLI Session

```text
🔐 Şifrenizi girin: deneme123
⚠️ Şifreniz zayıf. Güç seviyesi: 2/4

💡 Güçlü şifre oluşturmak için tercihlerinizi belirtin:
👉 Küçük harf olsun mu? (e/h): e
👉 Büyük harf olsun mu? (e/h): e
👉 Rakam olsun mu? (e/h): e
👉 Özel karakter (!,?,%) olsun mu? (e/h): e
👉 Şifre uzunluğu kaç karakter olsun? (örn: 12): 14

🔒 Önerilen güçlü şifre: Z!3eGv9u@K#p2Lm
```

---

## Author

**Mevlana Mert Çarlı**  
- GitHub: [@mert-carli](https://github.com/mert-carli)  
- Portfolio: [mert-carli-cvu9.vercel.app](https://mert-carli-cvu9.vercel.app)
