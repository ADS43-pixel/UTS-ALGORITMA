# UTS-ALGORITMA
Membuat program bank sampah sederhana

import os

loop = True

while loop:
	def menu() :
		print("\n-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+")
		print("BANK SAMPAH ZERO WASTE INDONESIA!")
		print("-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+")
		print("1. Menu Admin")
		print("2. Menu Setor Sampah")
		print("\n------------------------------------------")
		
	def pesan():
		jmlh_setor = int(input("Masukan jumlah sampah dalam pcs  : "))
		num_array = list()
		num = input("Berapa orang yang menyetor sampah ? : ")
		print ("Masukkan nama penyetor : ")
		for i in range (int(num)):
			i += 1
			n = input("orang ke {} :".format(i))
			num_array.append(str(n)) 
		total_uang = jmlh_setor*harga
		print("\n----------------------------------------------")
		print("Anda telah berhasil melakukan penyetoran sampah ")
		print("----------------------------------------------")
		print ("Nama penyetor :".format(len(num_array)))
		for a in num_array:
			print (("- {}").format(a))
		print("Uang sampah yang diterima","Rp.",(total_uang))


	menu()
	pilihan = int(input("Masukan Pilihan [1-2] : "))

	if ((pilihan) == 1):
		print("\n-------------------------------------------------------")
		print("\nINFORMASI JENIS SAMPAH DAN HARGA")
		print("\nPlastik kemasan belum digunting per pcs = Rp1.000")
		print("\nPlastik kemasan sudah digunting per pcs = Rp2.000")
		print("\nPlastik kemasan sudah dianyam per 100 sudut = Rp5.000")
		print("\nPlastik kemasan satu botol 500 ml = Rp1.500")
			
			
	elif ((pilihan) == 2):

		print("\n----------------------------------------")
		print("\nKode  Sampah\tBentuk\t\tTotal")
		print("\n      Plastik\tSampah\t\tHarga")
		print("\n----------------------------------------")
		print("\n101.  plastik biasa\tsampah kemasan \tRp1.000")
		print("\n102.  plastik guntingan\tsampah kemasan \tRp2.000")
		print("\n103.  plastik dianyam\tsampah kemasan \tRp5.000")
		print("\n104.  plastik botolan\tsampah kemasan \tRp1.500")
		print("\n---------------------------------------------")
		no_sampah = int(input("Masukkan kode sampah : "))
		
		if ((no_sampah) == 101):
			harga = 1000
			print("")
			print("---------------------------------")
			print("Anda memilih kode sampah",+int(no_sampah))
			print("---------------------------------")
			pesan()
			
		elif ((no_sampah) == 102):
			harga = 2000
			print("")
			print("---------------------------------")
			print("anda memilih kode sampah",+int(no_sampah))
			print("---------------------------------")
			pesan()
			
		elif ((no_sampah) == 103):
			harga = 5000
			print("")
			print("---------------------------------")
			print("anda memilih kode sampah",+int(no_sampah))
			print("---------------------------------")
			pesan()

		elif ((no_sampah) == 104):
			harga = 1500
			print("")
			print("---------------------------------")
			print("anda memilih kode sampah",+int(no_sampah))
			print("---------------------------------")
			pesan()
			
		else :
			print("kode bus tidak ada dalam daftar")
			
			
			
	
