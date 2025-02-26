# Hello-World
berisi program latihan di RWID as a DA
Ada program latihan untuk bikin menu
shopping_list = []

def tampilan_data():
  shopping_list = []

def tambah_data():
  nama_barang = input("Masukkan nama barang: ")
  jumlah_barang = int(input("Masukkan jumlah barang: "))
  shopping_list.append({nama_barang: jumlah_barang})
  print(f"Nama barang {nama_barang} berhasil ditambahkan")

def tampilan_data():
  if not shopping_list:
    print("Tidak ada data dalam daftar belanja")
  else:
    print("Daftar Belanja:")
    for item in shopping_list:
      for nama_barang, jumlah_barang in item.items():
        print(f"- {nama_barang}: {jumlah_barang}")
main_program = True
while main_program:
  print("\nMenu:")
  print("1. Tambah Data")
  print("2. Tampilan Menu")
  print("3. Keluar")
  pilihan = input("Pilih 1/2/3: ")
  if pilihan == "1":
    tambah_data()
  elif pilihan == "2":
    tampilan_data()
  elif pilihan == "3":
    print("Trimakasih")
    main_program = False
  else:
      print("Pilihan tidak valid, pilih lagi")
      main_program = True


