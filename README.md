
# MXChecker ⚔️🛡️ - Fast and Powerful Email Validator (KnightPentest)

**MXChecker** is a high-speed, cross-platform tool fully written in **Go** by the elite cybersecurity team, **KnightPentest**. It is designed to help you validate email addresses by checking their MX records. Simply input an email, like `test@example.com`, and receive a `good` or `bad` status in the logs.

## ✨ Features
- **Blazing Fast:** Leverages Go's concurrency to provide quick and reliable email validation.
- **Cross-Platform:** Works seamlessly on **Linux**, **Windows**, and **macOS**.
- **Multi-Threading:** Configure the number of threads (workers) in the `.env` file to match your needs.
- **No Proxy Required:** Run validations without the need for a proxy, though you can specify user agents.
- **Log Outputs:** Generates detailed logs for both successful and failed email checks.

## 📦 How to Use

### 🐧 On Linux/macOS
1. Extract all files into a separate folder.
2. Edit the `.env` file to suit your configuration:
   - Specify the file containing the emails.
   - Set the number of workers (threads).
   - Optionally, configure user agents.
   - Place all files in the same folder as the binary.
3. Run the command:
   ```bash
   ./mxchecker
   ```
   ![Linux/macOS Usage](https://github.com/user-attachments/assets/ea24ffc1-cfe6-4436-a4dc-55beae2b2aae)
4. Check the logs generated in the same folder as `mxchecker`.

### 🪟 On Windows
1. Create an `.env` file in the same directory as `mxchecker.exe`:
   ```powershell
   New-Item -Path "C:\Users\username\Desktop\checker\.env" -ItemType File
   ```
2. Add the necessary content to `.env` (find the example in this repository's source files).
3. In `cmd`, navigate to the directory:
   ```cmd
   cd C:\Users\username\Desktop\checker
   ```
   ![Windows Usage](https://github.com/user-attachments/assets/a0f00de4-dc9b-4f08-bb82-067f1bf61f85)
4. Run the checker:
   ```cmd
   mxchecker.exe
   ```
5. Results are saved in logs with the format: `logs_year-month-day_hour-minute`.

## 🛠️ Configuration
- Modify `.env` to control worker threads and specify input email files.
- Ensure all required files (`.env`, user agents) are in the same folder as the binary.

## 🤝 Crafted by KnightPentest
**KnightPentest** is not just a team; it's a brotherhood of elite cybersecurity experts. **MXChecker** reflects our commitment to creating fast, reliable, and easy-to-use tools for the cybersecurity community.

## 🔥 Get Started
Extract, configure, and run **MXChecker** today to quickly validate emails with ease!
