```mermaid
flowchart LR
    budi["aguz : Penghuni<br/>nama = Aguz"]
    k01["k01 : Kamar<br/>nomorKamar = A-01<br/>status = Terisi"]
    dt01["dt01 : DigitalTwin<br/>suhu = 28 °C<br/>kelembapan = 65 %<br/>statusLampu = AKTIF<br/>kondisiSuhu = Normal<br/>kondisiKelembapan = Normal"]
    s01["s01 : SensorDHT22<br/>suhu = 28 °C<br/>kelembapan = 65 %"]
    l01["l01 : Lampu<br/>status = AKTIF (Menyala)"]

    budi -- "menempati" --> k01
    k01 -- "memiliki" --> dt01
    s01 -- "kirim data" --> dt01
    dt01 -- "status" --> l01
```

# Object Diagram - Digital Twin Kamar Kos

```mermaid
classDiagram
    direction TB

    class Budi["Budi : Penghuni"] {
        id = P001
        nama = Budi Santoso
        noHP = 081234567890
    }

    class KamarA01["A01 : Kamar"] {
        noKamar = A01
        lantai = 1
        hargaSewa = 1200000
        status = Terisi
    }

    class Esp32["ESP32-A01 : PerangkatESP32"] {
        deviceId = ESP32-A01
        protokol = MQTT
        ipAddress = 192.168.1.21
        status = Online
    }

    class Dht22["DHT22-A01 : SensorDHT22"] {
        sensorId = DHT-A01
        suhu = 28.5 °C
        kelembapan = 62 %
        kondisiSuhu = Normal
        kondisiKelembapan = Normal
    }

    class Lampu["Lampu-A01 : Lampu"] {
        lampuId = L-A01
        status = AKTIF
        mode = Manual
    }

    class Log["Log-0001 : DataSensor"] {
        logId = 0001
        waktu = 25/10/2026 14:59
        suhu = 28.5
        kelembapan = 62
    }

    Budi -- KamarA01
    KamarA01 -- Esp32
    Esp32 -- Dht22
    KamarA01 -- Lampu
    Lampu -- Log
```
