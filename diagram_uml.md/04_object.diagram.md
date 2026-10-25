# Object Diagram - Digital Twin Kamar Kos

```mermaid
classDiagram
    direction TB
    class agusz["agusz : Penghuni"] {
        id = P002
        nama = Agusz Nugraha
        noHP = 085142219806
    }
    class KamarA01["A01 : Kamar"] {
        noKamar = A02
        lantai = 2
        hargaSewa = 575.000
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

    Aguz -- KamarA01
    KamarA01 -- Esp32
    Esp32 -- Dht22
    KamarA01 -- Lampu
    Lampu -- Log
```
