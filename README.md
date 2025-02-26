# Hello-World
berisi program latihan di RWID as a DA
Pada program tambah barang, jumlah barang diprotek tidak boleh nol
ganti fungsi tambah_data dengan code berikut

def tambah_data():
  while True:
    try:
      nama_barang = input("Masukkan nama barang: ")
      jumlah_barang = int(input("Masukkan jumlah barang: "))
      if jumlah_barang == 0:
        raise ValueError("Jumlah barang minimal 1")
      shopping_list.append({nama_barang: jumlah_barang})
      print(f"Nama barang {nama_barang} berhasil ditambahkan")
      break    #keluar dr loop
    except ValueError as e:
      print(e)    #print error
