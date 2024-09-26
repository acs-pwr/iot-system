# IOT System

## Use Case
#### EPIC 1 : Sub Sistem Perangkat IoT
- Sistem memiliki  sensor-sensor lingkungan berupa  suhu lingkungan, kelembaban lingkungan, intensitas cahaya lingkungan dan mengambil gambar lingkungan
- Sistem dapat mendeteksi suhu lingkungan
- Sistem dapat mendeteksi intensitas cahaya lingkungan
- Sistem dapat mendeteksi kelembaban udara lingkungan
- Sistem dapat mendeteksi mengambil gambar kondisi perangkat serangga
- Sistem dapat mengisi daya dari solar panel

#### EPIC 1 : Sub Sistem Komunikasi
- Sistem memiliki  modem 4G untuk mengirim data sensor-sensor pada Sub Sistem Perangkat IOT yaitu data intensitas cahaya lingkungan, data suhu lingkungan, data kelembaban udara lingkungan dan mengambil gambar lingkungan
- Sistem dapat mengirim data dari sensor suhu lingkungan
- Sistem dapat mengirim data dari sensor intensitas cahaya lingkungan
- Sistem dapat mengirim data dari sensor kelembaban udara lingkungan
- Sistem dapat mengirim data dari sensor mengambil gambar kondisi perangkat serangga
- Sistem dapat mengirim data nomor pengenal perangkat IOT ke Subsistem Back End
- Sistem dapat mengirim data mengenai status aktif atau tidak perangkat IOT
- Sistem dapat menerima perintah berupa data dari Sub Sistem back end untuk mengaktifkan sensor lingkungan.
- Sistem dapat menggunakan protokol MQTT atau http untuk mengirim data dari sensor ke Subsistem Back End

#### EPIC 2 : Sub Sistem Back End
- Sistem menerima data sensor-sensor pada Sub Sistem Perangkat IOT yaitu data intensitas cahaya lingkungan, data suhu lingkungan, data kelembaban udara lingkungan dan mengambil gambar lingkungan
- Sistem dapat menerima dan menyimpan data dari sensor suhu lingkungan dari Subsistem Perangkat IOT
- Sistem dapat menerima dan menyimpan data dari sensor intensitas cahaya lingkungan dari Subsistem Perangkat IOT
- Sistem dapat menerima dan menyimpan data dari sensor kelembaban udara lingkungan dari Subsistem Perangkat IOT
- Sistem dapat menerima dan menyimpan dari sensor pengambil gambar kondisi perangkat serangga dari Subsistem Perangkat IOT
- Sistem menerima dan menyimpan data nomor pengenal perangkat IOT ke Sub Sistem Back End 
- Sistem menerima dan menyimpan mengenai status aktif atau tidak perangat IOT
- Sistem menerima dan menyimpan berupa data dari Sub Sistem back end untuk mengaktifkan sensor-sensor lingkungan dari Sub Sistem Perangkat IOT.
- Sistem dapat menggunakan protokol MQTT atau http untuk menerima dan menyimpan data dari sensor-sensor dari Sub Sistem Perangkat IOT
- Sistem dapat mengirim dan mengolah data dari sensor suhu lingkungan dari Subsistem Perangkat IOT ke Sub Sistem Aplikasi Front End
- Sistem mengirim dan mengolah data data dari sensor intensitas cahaya lingkungan dari Subsistem Perangkat IOT ke Sub Sistem Aplikasi Front End
- Sistem dapat mengirim dan mengolah data data dari sensor kelembaban udara lingkungan dari Subsistem Perangkat IOT ke Sub Sistem Aplikasi Front End
- Sistem dapat mengirim dan mengolah data dari sensor pengambil gambar kondisi perangkat serangga dari Subsistem Perangkat IOT ke Sub Sistem Aplikasi Front End
- Sistem dapat menyimpan gambar ke Object Storage
- Sistem dapat menyimpan data ke DataBase Postgres

### EPIC 2 : Sub Sistem Front End
- Sistem dapat menampilkan data dari sensor suhu lingkungan dari Subsistem Perangkat IOT
- Sistem dapat dapat menampilkan data dari sensor intensitas cahaya lingkungan yang dikirim dari Subsistem Back End
- Sistem dapat menerima dan menyimpan data dari sensor kelembaban udara lingkungan yang dikirim dari Subsistem Back End
- Sistem dapat menerima dan menyimpan dari sensor pengambil gambar kondisi perangkat serangga yang dikirim dari Subsistem Back End
- Sistem menerima dan menyimpan data nomor pengenal perangkat IOT yang dikirim dari Subsistem Back End
- Sistem menerima dan menyimpan mengenai status aktif atau tidak perangkat IOT yang dikirim dari data Subsistem Back End
- Sistem menerima dan menyimpan berupa data dari Sub Sistem back end untuk mengaktifkan sensor-sensor lingkungan dari data  yang dikirim dari Subsistem Back End.
- Sistem dapat menggunakan protokol MQTT atau http untuk menerima dan menyimpan data dari data yang dikirim dari Subsistem Back End
- Sistem menampilkan hasil olahan data dari sensor suhu lingkungan dari hasil pengolahan Subsistem Back End
- Sistem menampilkan data data dari sensor intensitas cahaya lingkungan dari hasil pengolahan Subsistem Back End
- Sistem menampilkan data data dari sensor kelembaban udara lingkungan dari Subsistem Perangkat IOT ke Sub Sistem Aplikasi Front End
- Sistem dapat menampilkan dari sensor pengambil gambar kondisi perangkat serangga dari data yang dikirim Subsistem Back End
- Sistem dapat menampilkan gambar dari Object Storage
- Sistem dapat menampilkan data dari DataBase Postgres
- Sistem Dapat menampilkan grafik hasil sensor suhu , kelembapan , intensitas cahaya berdasar filter jangka waktu tertentu seperti harian, jam, mingguan
- Sistem Dapat menampilkan grafik hasil sensor suhu , kelembapan , intensitas cahaya berdasar filter lokasi perangkat iot dalam bentuk peta
- Sistem Dapat menampilkan grafik hasil sensor suhu , kelembapan , intensitas cahaya berdasar filter identitas pengangkat IOT
- Sistem dapat menampilkan notifikasi mengenai keaktifan dari perangkat IOT apakah kondisi aktif atau non aktif
- Sistem dapat menampilkan notifikasi mengenai adanya data baru dari sensor lingkungan perangkat IOT yang masuk ke Sistem. 
- Sistem dapat mengirim data ke Sub Sistem Back End untuk mengaktifkan Sensor Lingkungan di perangkat IOT
- Sistem dapat mengatur jadwal mengirim data ke Subsistem Back End untuk mengaktifkan Sensor Lingkungan di perangkat IOT contoh jadwal jam , harian, mingguan , etc
- Sistem dapat menambahkan data perangkat IOT yang  mengirim data dari sensor-sensor lingkungan ke Subsistem Back End.
- Sistem dapat menambah, mengedit dan menghapus data foto untuk koleksi foto serangga yang dikirimkan ke Sub Sistem Back End
- Sistem dapat mengatur hak akses berdasar Role Based Access Control

## Mind Map
[Miro](https://miro.com/app/board/uXjVLaXDEdE=/?share_link_id=688206844644)

## User Story 
Sebagai pengguna IoT,
Saya ingin memantau kondisi lingkungan melalui sensor,
Sehingga saya dapat mengambil tindakan yang diperlukan berdasarkan data yang dikumpulkan.

## Acceptance Criteria

1.  Sensor harus dapat mendeteksi suhu, kelembaban, dan intensitas cahaya.
    -   Data yang dikumpulkan harus akurat dan dapat diakses oleh sistem.
2.  Data sensor harus dikirim ke Sub Sistem Back End secara real-time.
    -   Data dikirim menggunakan protokol MQTT atau HTTP.
3.  Back End harus menyimpan data sensor dan gambar dengan benar.
    -   Data yang disimpan harus bisa diakses kembali tanpa kehilangan informasi.
4.  Frontend harus menampilkan data secara real-time dan memberi notifikasi.
    -   Pengguna harus menerima notifikasi ketika ada data baru atau status perangkat berubah.

## Test Case

```
Feature: IoT System Sensor Functionality

  Scenario: Detect environmental temperature
    Given the temperature sensor is operational
    When the sensor measures the temperature
    Then the system should display the temperature data

  Scenario: Detect environmental humidity
    Given the humidity sensor is operational
    When the sensor measures the humidity level
    Then the system should display the humidity data

  Scenario: Detect environmental light intensity
    Given the light intensity sensor is operational
    When the sensor measures the light intensity
    Then the system should display the light intensity data

  Scenario: Capture image of the environment
    Given the image capture sensor is operational
    When the sensor captures an image
    Then the system should store the image correctly

  Scenario: Powering up using solar panel
    Given the solar panel is connected to the system
    When the system requires charging
    Then the system should utilize the solar panel for power

Feature: IoT Communication System

  Scenario: Send temperature data to Back End
    Given the temperature data is available
    When the data is sent using MQTT
    Then the Back End should receive and store the temperature data

  Scenario: Send humidity data to Back End
    Given the humidity data is available
    When the data is sent using HTTP
    Then the Back End should receive and store the humidity data

  Scenario: Send device identification to Back End
    Given the device identification number is available
    When the identification is sent
    Then the Back End should store the device identification

Feature: Back End Data Management

  Scenario: Receive and store sensor data
    Given the Back End is operational
    When the sensor data is received
    Then the Back End should save the data in the database

  Scenario: Process and send data to Front End
    Given the sensor data is stored
    When the Front End requests data
    Then the Back End should send the appropriate data

Feature: Front End Display Functionality

  Scenario: Display temperature data
    Given the temperature data is available from Back End
    When the Front End retrieves the data
    Then the Front End should display the temperature information

  Scenario: Display notification for new sensor data
    Given new sensor data has been received
    When the notification is triggered
    Then the user should see the notification on the Front End

  Scenario: Display graph of sensor data
    Given the sensor data is available
    When the user selects a time filter
    Then the system should display the graph based on the selected time range

```
