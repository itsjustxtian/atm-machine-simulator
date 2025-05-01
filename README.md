# CPE 460 Final Project: ATM Simulator

This project is a simple ATM simulator written in Assembly Language for the 8086 microprocessor. It supports:

- User login with encrypted password
- Viewing current balance
- Depositing funds
- Withdrawing funds
- Basic security and encryption using XOR

---

## 💻 Requirements

- **EMU8086** (or any 8086-compatible assembler/emulator)

You can download EMU8086 [here.](https://emu8086.en.lo4d.com/windows)

---

## 🚀 How to Run

1. Open EMU8086.
2. Copy and paste the contents of the `.asm` file into a new `.asm` file.
3. Click **Assemble** then **Run**.
4. Follow the prompts in the console.

---

## 🧾 Example Login

To simplify the login process, all users up to user 15 have the same password as their ID number. For example: `ID: 0` has a password of `0` as well, up until user 15. Users 16 to 19 restart their passwords back to 1 to 4, respectively.

> Passwords are encrypted using XOR with the key `5Ah`.

---

## 🧠 Features

- 🔐 XOR-based encryption on password input
- 💰 Balance management system (each user starts with 1000)
- 📋 Menu options for:
  - Check Balance
  - Deposit
  - Withdraw
  - Exit
- 🧠 Index-based user tracking
