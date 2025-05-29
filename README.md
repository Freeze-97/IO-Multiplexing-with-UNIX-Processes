# 💻 I/O Multiplexing with UNIX Processes

## 📖 Description

This project demonstrates UNIX I/O concepts, specifically focusing on I/O multiplexing using select()/poll(), pipes, and parent-child process communication. The lab task explores inter-process communication where two child processes compute digits of π (pi) and e (Euler’s number), sending their results to a parent process via pipes.

The parent process:

Monitors the child processes using poll().

Writes received digits to separate files (pi.dat and e.dat).

Periodically outputs statistics for every 1000 digits received from each child.

## 🛠️ Compilation

To compile the program:
```bash
To compile the program:
```
This will generate the executable

## ▶️ Usage
```bash
./lab2 [number_of_digits]
```
If no argument is provided, the default is 50000 digits.

## 🧪 Output
- The program writes the computed digits to:

  - pi.dat (digits of π)

  - e.dat (digits of e)

- Every 1000 digits, it prints a distribution summary of the digits (0–9) for π and e to stdout.

- It also outputs the status of each child process when they finish.

## 📌 Requirements
- UNIX-based operating system (e.g., Linux or macOS)

- g++ compiler

- Make utility
