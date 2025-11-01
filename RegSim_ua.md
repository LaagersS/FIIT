# RegSim на macOS (ARM/Intel)

## Крок 1: Перевір наявність Java
````bash
java -version
````

Якщо Java немає, встанови:

```bash
brew install --cask temurin
```

## Крок 2: Підготуй папку для RegSim

Створи папку де хочеш зберігати RegSim:

```bash
mkdir -p ТВОЯ_ПАПКА_ДЕ_БУДЕ_REGSIM
```

Помісти туди `regsim.jar` (завантаж з [https://www2.fiit.stuba.sk/~kristofik/other_en.html](https://www2.fiit.stuba.sk/~kristofik/other_en.html))

Перевір що файл на місці:

```bash
ls -la ТВОЯ_ПАПКА_ДЕ_БУДЕ_REGSIM
```

## Крок 3: Завантаж JavaFX SDK

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

## Крок 4: Запусти RegSim

```bash
cd ТВОЯ_ПАПКА_ДЕ_БУДЕ_REGSIM
java --module-path ./javafx-sdk-21.0.1/lib --add-modules javafx.controls,javafx.fxml,javafx.graphics,javafx.swing -jar regsim.jar
```
