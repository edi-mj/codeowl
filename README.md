# Code Owl

![Construct 2](https://img.shields.io/badge/Construct_2-00ADD8?style=flat-square&logo=construct3&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![WebGL](https://img.shields.io/badge/WebGL-990000?style=flat-square&logo=webgl&logoColor=white)
![JSON](https://img.shields.io/badge/JSON-000000?style=flat-square&logo=json&logoColor=white)

**Code Owl** adalah game edukasi interaktif yang mengajarkan dasar-dasar pemrograman Python melalui puzzle berbasis grid. Dikembangkan menggunakan Construct 2, game ini memadukan pembelajaran coding dengan gameplay yang engaging.

## Demo

Coba game secara langsung di: [edi-mj.github.io/codeowl/](https://edi-mj.github.io/codeowl/)

## Tentang Proyek

Code Owl dirancang untuk pemula yang ingin belajar konsep fundamental Python dengan cara yang menyenangkan. Pemain akan menulis kode sederhana untuk menggerakkan karakter melewati berbagai rintangan dan mencapai tujuan.

### Materi Pembelajaran

- **Variabel & Assignment** - Deklarasi dan pengisian nilai variabel
- **Tipe Data Integer** - Bekerja dengan angka
- **Function Calls** - Memanggil method dengan parameter
- **Sequential Logic** - Memahami urutan eksekusi kode
- **Control Flow** - Logika dasar pemrograman

## Fitur Utama

### Sistem Level Progresif

Game terdiri dari multiple chapter dengan tingkat kesulitan yang meningkat secara bertahap. Setiap level memiliki objectives yang jelas dan hint untuk membantu pemain.

### Progress Tracking

Sistem save otomatis menggunakan browser local storage, memungkinkan pemain melanjutkan progress kapan saja.

### Code Editor Interface

Interface yang sederhana dan intuitif memudahkan pemain untuk menulis kode tanpa distraksi berlebihan.

## Teknologi

### Game Engine

- **Construct 2** - Visual game development platform untuk HTML5

### Plugins & Libraries

- **AJAX** - Loading data level dari JSON
- **JSON Parser** (Yann Granjon) - Parse konfigurasi level
- **Local Storage** - Menyimpan progress pemain
- **Web Font Loader** (Rex.Rainbow) - Custom typography
- **LiteTween** (lunarray) - Smooth animations
- **MoveTo & RotateTo** (Rex.Rainbow) - Character movement behaviors

### Assets

- Environment tiles (tanah, air, batu, jembatan, dll) - [CraftPix Free Level Map Pixel Art Assets Pack](https://craftpix.net/freebies/free-level-map-pixel-art-assets-pack/)
- Custom sprite untuk characters dan interactive objects
- Sound effects dan background music
- 10,000+ baris level configuration dalam JSON format

## Cara Menjalankan

### Menggunakan Construct 2

1. Install [Construct 2](https://www.construct.net/en/construct-2) (versi 280 atau lebih baru)
2. Buka file `main.capx`
3. Klik tombol "Run layout" untuk preview

### Dari Source Code

1. Extract file `main.capx` (format ZIP)
2. Buka `Code Owl.caproj` di Construct 2
3. Export sebagai HTML5 project
4. Host file HTML di web server atau buka langsung di browser

## Contoh Level

**Level 1 - "Tinggal Lurus"**

```python
langkah = 7
player.step(langkah)
```

Pemain harus mengisi variabel `langkah` dengan nilai yang tepat.

**Level Lanjutan**

```python
player.step(4)
player.turn("left")
player.step(1)
Jembatan = 50
player.step(10)
player.turn("left")
player.step(17)
```

Kombinasi movement commands dan variable assignment.

## Game Mechanics

### Commands Tersedia

- `player.step(n)` - Gerakkan karakter sebanyak n langkah
- `player.turn(direction)` - Putar karakter ("left", "right", dll)
- Variable assignment - Buka obstacle dengan nilai yang tepat

### Objects

- **Player** - Karakter yang dikendalikan player
- **Portal** - Tujuan akhir setiap level
- **Wall** - Penghalang statis
- **Bridge/Gate** - Rintangan yang memerlukan variabel untuk dibuka
- **Crystal/Beacon** - Collectibles opsional

## Browser Compatibility

Game ini dioptimalkan untuk browser modern dengan dukungan:

- HTML5 Canvas
- WebGL
- Web Audio API
- LocalStorage API

Tested on: Chrome, Firefox, Edge, Safari

## Target Platform

- **Platform:** Web Browser (HTML5)
- **Resolution:** 1536 x 736 pixels
- **Orientation:** Landscape
- **Input:** Mouse/Touch

## Development Notes

Project ini menggunakan Construct 2 event system untuk logika game, yang memungkinkan development visual tanpa coding tradisional. Namun, game ini sendiri mengajarkan konsep coding kepada end user.

Level configuration disimpan dalam format JSON untuk memudahkan editing dan penambahan level baru tanpa perlu membuka project file.

## Contributing

Contributions welcome! Beberapa area yang bisa dikembangkan:

- Menambah level baru dengan konsep Python yang lebih advanced
- Improve UI/UX untuk code editor
- Menambah materi pembelajaran (loops, conditionals, etc)
- Localization ke bahasa lain

## License

Project ini dibuat untuk tugas akhir mata kuliah Pengembangan Perangkat Lunak.

## Credits

- Game Design & Development: Original team
- Sound Effects: Game audio assets
- BGM: "Whispering Pines", "Pixel Forest Dream"

---

**Note:** File `.capx` adalah format proprietary Construct 2 yang merupakan archive ZIP berisi XML dan asset files.
