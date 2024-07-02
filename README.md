# Sinhala Keyboard (Hela) Transliteration Scheme

The "Sinhala Keyboard (Hela) Transliteration Scheme" provides a comprehensive guide for typing Sinhala characters using a standard QWERTY keyboard. It includes tables for vowels, consonants, and consonant clusters, detailing both independent and dependent forms. This scheme is designed to simplify the typing process by using Latin alphabet keys, with a preference for lowercase, uppercase, and ALT-GR keys. The document also includes special notes on key functions and provides an implementation link for practical use. This scheme aims to facilitate efficient and accurate Sinhala text input for users familiar with the Latin keyboard layout.

## Vowels

| Independent |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
|-------------|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|
| අ           | ආ | ඇ | ඈ | ඉ | ඊ | උ | ඌ | ඍ | ඎ | ඏ | ඐ | එ | ඒ | ඓ | ඔ | ඕ | ඖ |   | ‌ං | ‌ඃ |
| a           | aa | A | AA | i | ii | u | uu | R | Ru | LU | LUU | e | ee | ai | o | oo | au |   | x | H |

| Dependent   |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
|-------------|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|--|
| ක           | කා | කැ | කෑ | කි | කී | කු | කූ | කෘ | කෲ | කෟ | කෳ | කෙ | කේ | කෛ | කො | කෝ | කෞ | ක් | කං | කඃ |
| ka          | kaa | kA | kAA | ki | kii | ku | kuu | krU | krUU | klU | klUU | ke | kee | kai | ko | koo | kau | k | kax | kaH |

## Consonants

| Voiceless |  | Voiced |  | Nasal | Nasalised Voiced |
|-----------|--|--------|--|-------|------------------|
| Velar     |  | Velar  |  | Velar | Velar            |
| ක         | ඛ | ග     | ඝ | ඞ   | ඟ              |
| ka        | kha | ga | gha | Xa | zga |

| Palatal |  | Palatal |  | Palatal | Palatal |
|---------|--|---------|--|---------|---------|
| ච       | ඡ | ජ     | ඣ | ඤ     | ඦ      |
| cha     | chha | ja | jHa | zka | zja |

| Alveolar |  | Alveolar |  | Alveolar | Alveolar |
|----------|--|----------|--|----------|----------|
| ට        | ඨ | ඩ     | ඪ | ණ     | ඬ       |
| ta       | Ta | da     | Da | Na     | zda      |

| Dental   |  | Dental  |  | Dental  | Dental   |
|----------|--|---------|--|---------|----------|
| ත        | ථ | ද     | ධ | න     | ඳ        |
| tha      | thha | dha | dhha | na | zdha |

| Bilabilal |  | Bilabilal |  | Bilabilal | Bilabilal |
|-----------|--|-----------|--|-----------|-----------|
| ප         | ඵ | බ       | භ | ම         | ඹ        |
| pa        | pha | ba     | bha | ma       | Ba        |

## Glides, Fricatives, etc

| ය         | ර   | ල  | ව  | ශ   | ෂ  | ස  | හ  | ළ  | ෆ  |
|-----------|-----|----|----|-----|----|----|----|----|----|
| ya        | ra  | la | va | sha | Sa | sa | ha | La | fa |

## Consonant Clusters

| ඥ         | ක්‍ර | ක්‍ය | ර්‍ක |
|-----------|-----|-----|-----|
| zha       | kqra | kqya | rqka |

## Note

- The key (q) is used to join letters.
- The key (Q) is used to create touching letters.
- (A-) represents ALT-GR. i.e. The right ALT key.
- Press (A-.) to insert a "෴".
- Press SHIFT-space to insert a no-break space.
- Press (A-space) to insert a ZWNJ.

## Objective

This (Hela) transliteration scheme is only for typing Sinhala words using a standard QWERTY keyboard. Only use the keys corresponding to the letters of the Latin alphabet. Give preference to lowercase keys, then uppercase keys and lastly ALT-GR. If ALT-GR is used, provide a non-ALT-GR input sequence to create the same Sinhala letter.

## Implementations

- [si-trans.mim (m17n)](./si-hela.mim)

---

## User Guide: on Linux (Debian/Ubuntu and Fedora)

Follow these steps to set up and use the `si-hela.mim` Sinhala transliteration keymap on your Linux system:

### 1. Locate the `si-hela.mim` File
Ensure you have the `si-hela.mim` file available on your system. If not, download [si-trans.mim (m17n)](./si-hela.mim) or obtain it from the source where it's provided.

### 2. Install the `ibus-m17n` Package
IBus (Intelligent Input Bus) is an input framework for Linux OS, and `ibus-m17n` integrates IBus with the M17N library for multilingual text processing.

#### On Debian/Ubuntu:
Install it using the following command:
```sh
sudo apt-get install ibus-m17n
```

#### On Fedora:
Install it using the following command:
```sh
sudo dnf install ibus-m17n
```

### 3. Copy the `si-hela.mim` File
Copy the `si-hela.mim` file to the directory where IBus searches for input method files, usually `/usr/share/m17n/`. Root permissions are required to copy the file:
```sh
sudo cp si-hela.mim /usr/share/m17n/
```

### 4. Restart IBus
Restart IBus to recognize the new input method:
```sh
ibus restart
```

### 5. Add the Input Method
Add the Sinhala transliteration input method to your IBus input sources through your system settings:
1. Go to "Region & Language" or "Keyboard Settings".
2. Add a new input source.
3. In the input sources list, find and add "Sinhala (hela transliteration)" or a similar option.

### 6. Switch Input Method
Switch to the Sinhala transliteration input method using the IBus menu or the shortcut keys configured in your system settings. You can now type Sinhala text using transliteration.

---

## Troubleshooting
If you encounter any issues, refer to the issue area for further assistance or consult community forums for additional help.


`started: 2024-06-25, last updated: 2024-06-26`
