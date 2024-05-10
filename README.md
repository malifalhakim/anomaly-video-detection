### Folder Checkpoint

Berisi weight dari model pytorch yang telah dilatih menggunkan main.py dan ditest pada test.py jika accuracy memenuhi standard tertentu. Weight ini dipindahkan ke folder VIS/weight untuk melakukan prediksi sekaligus visualisasi

### Folder UCF-Crime

Berisi dataset yang telah diekstrak fiturnya dengan mengambil fitur pada rgb+flows. File txt berguna meng-list nama file video

### Folder Vis

Secara umum berguna untuk menggunakan model (yang telah dilatih sebelumnya) untuk memprediksi dan memvisualisasikan video yang ingin diprediksi.

- File NamaVideo.mp4, seperti Abuse001_x264.mp4 merupakan raw video yang ingin diprediksi

- Folder NamaVideo merupakan frame hasil ekstrak menggunakan ffmpeg dari NamaVideo.mp4

- Folder models berisi arsitekstur model untuk fitur ekstraksi

- Folder PNG berisi hasil plot prediksi dari model
- Folder RE berisi setiap frame hasil prediksi

- Folder weight berisi weight model prediksi(ckpt.pth) dan model fitur ekstraksi

- File NamaVideo_result.mp4 berisi video hasil prediksi gabungan frame hasil prediksi

- File learner -> Arsitekstur model prediksi

- File video2frame -> mengubah video menjadi frame

- File vis -> melakukan prediksi dan visualisasi

### Root Folder

- File dataset -> Kode untuk objek dataset loader
- File FFC -> Learner versi ke 2 (klasifikasi)
- File learner dan learner2 -> Arsitektur Learner (terkait dengan model prediksi)
- File loss -> Loss function untuk melatih model
- File main -> Untuk melatih model dan memprediksi
- File test -> Untuk melakukan prediksi pada test dataset
