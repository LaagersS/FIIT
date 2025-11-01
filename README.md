# Сontent

* [RegSim](#regsim)
  * [English](#regsim-on-macos-armintel)
  * [Українська](#regsim-на-macos-armintel)
* [LogiSim](#logisim)

---

# RegSim

## RegSim on macOS (ARM/Intel)

### Step 1: Check for Java

```bash
java -version
```

If Java is not installed, install it:

```bash
brew install --cask temurin
```

### Step 2: Prepare a folder for RegSim

Create a folder where you want to store RegSim:

```bash
mkdir -p YOUR_FOLDER_FOR_REGSIM
```

Place `regsim.jar` there (download from [https://www2.fiit.stuba.sk/~kristofik/other_en.html](https://www2.fiit.stuba.sk/~kristofik/other_en.html)).

Check that the file is in place:

```bash
ls -la YOUR_FOLDER_FOR_REGSIM
```

### Step 3: Download JavaFX SDK

Go to the folder with RegSim:

```bash
cd YOUR_FOLDER_FOR_REGSIM
```

**For ARM Mac (M1/M2/M3):**

```bash
curl -L -O https://download2.gluonhq.com/openjfx/21.0.1/openjfx-21.0.1_osx-aarch64_bin-sdk.zip
unzip openjfx-21.0.1_osx-aarch64_bin-sdk.zip
```

**For Intel Mac:**

```bash
curl -L -O https://download2.gluonhq.com/openjfx/21.0.1/openjfx-21.0.1_osx-x64_bin-sdk.zip
unzip openjfx-21.0.1_osx-x64_bin-sdk.zip
```

**Not sure which Mac you have?** Run:

```bash
uname -m
```

* `arm64` = ARM (M-series)
* `x86_64` = Intel

### Step 4: Run RegSim

```bash
cd YOUR_FOLDER_FOR_REGSIM
java --module-path ./javafx-sdk-21.0.1/lib --add-modules javafx.controls,javafx.fxml,javafx.graphics,javafx.swing -jar regsim.jar
```

---

## RegSim на macOS (ARM/Intel)

### Крок 1: Перевір наявність Java

```bash
java -version
```

Якщо Java немає, встанови:

```bash
brew install --cask temurin
```

### Крок 2: Підготуй папку для RegSim

Створи папку де хочеш зберігати RegSim:

```bash
mkdir -p ТВОЯ_ПАПКА_ДЕ_БУДЕ_REGSIM
```

Помісти туди `regsim.jar` (завантаж з [https://www2.fiit.stuba.sk/~kristofik/other_en.html](https://www2.fiit.stuba.sk/~kristofik/other_en.html))

Перевір що файл на місці:

```bash
ls -la ТВОЯ_ПАПКА_ДЕ_БУДЕ_REGSIM
```

### Крок 3: Завантаж JavaFX SDK

Перейди в папку з RegSim:

```bash
cd ТВОЯ_ПАПКА_ДЕ_БУДЕ_REGSIM
```

**Для ARM Mac (M1/M2/M3):**

```bash
curl -L -O https://download2.gluonhq.com/openjfx/21.0.1/openjfx-21.0.1_osx-aarch64_bin-sdk.zip
unzip openjfx-21.0.1_osx-aarch64_bin-sdk.zip
```

**Для Intel Mac:**

```bash
curl -L -O https://download2.gluonhq.com/openjfx/21.0.1/openjfx-21.0.1_osx-x64_bin-sdk.zip
unzip openjfx-21.0.1_osx-x64_bin-sdk.zip
```

**Не знаєш який у тебе Mac?** Виконай:

```bash
uname -m
```

* `arm64` = ARM (M-series)
* `x86_64` = Intel

### Крок 4: Запусти RegSim

```bash
cd ТВОЯ_ПАПКА_ДЕ_БУДЕ_REGSIM
java --module-path ./javafx-sdk-21.0.1/lib --add-modules javafx.controls,javafx.fxml,javafx.graphics,javafx.swing -jar regsim.jar
```

---

# LogiSim 

### English

Step 1: Install LogiSim: [LINK](https://sourceforge.net/projects/circuit/)

Step 2: Launch: Unfortunately, when trying to run Logisim.app, you may encounter an error. To fix it, watch this [video](https://www.youtube.com/watch?v=7-HfWImd_0E)

### Українська

Крок 1: Встанови LogiSim: [LINK](https://sourceforge.net/projects/circuit/)

Крок 2: Запуск: На жаль, при спробі запуску Logisim.app, ви отримаєте помилку. Для її фіксу дивіться [відео](https://www.youtube.com/watch?v=7-HfWImd_0E)
