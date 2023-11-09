# Perpustakaan web sederhana BukuKita 

### menggunakan
 - html
 - css tailwind
 - javascript 


### cara membuat

1. buat file html serperti pada umumnya
2. jangan lupa masukan link cdn tailwind
   ```js
   <script src="https://cdn.tailwindcss.com"></script>
   ```
3. kita buat navbar terlebih dahulu
```js
 <nav class="bg-white border-2 w-full py-2">
      <div class="container mx-auto px-4 sm:px-12 lg:px-28 flex justify-between items-center">
        <a href="#">
          <div class="flex items-center">
            <img src="img/logo.jpg" alt="logo" class="w-14 cursor-pointer" />
            <p class="text-2xl mt-3 font-semibold text-blue-800">BukuKita.com</p>
          </div>
        </a>
        <ul class="flex text-center pt-3 space-x-4">
          <li class="list-none">
            <a href="#" class="text-blue-800 font-semibold no-underline" onclick="info()">Kategori</a>
          </li>
          <li class="list-none">
            <a href="#" class="text-blue-800 font-semibold no-underline" onclick="info()">Download</a>
          </li>
          <li class="list-none">
            <a href="#" class="text-blue-800 font-semibold no-underline" onclick="info()">Contact</a>
          </li>
        </ul>
      </div>
    </nav>
```

4. lalu kita lanjut untuk bagian setelah navbar adalah isi webnya daftar buku 
```js
<main>
      <div class="flex justify-between">
        <h1 class="text-3xl font-semibold px-28 mt-10">Rekomendasi buku</h1>
        <button type="button" onclick="lainnya()" class="px-28 mt-16 text-blue-800">lihat semua</button>
      </div>
      <div class="flex px-28">
        <!-- 1 -->
        <div class="w-1/4 mx-auto p-4 mt-4">
          <a href="#">
            <div class="bg-white shadow-lg p-4">
              <img src="https://www.gramedia.com/blog/content/images/2023/04/11.jpg" alt="Buku 2" class="w-36 h-48 mx-auto" />
              <p class="text-lg font-semibold mt-4 text-neutral-600">Seni Berbicara</p>
            </div>
          </a>
        </div>
        <!-- 2 -->
        <div class="w-1/4 mx-auto p-4 mt-4">
          <a href="#">
            <div class="bg-white shadow-lg p-4">
              <img src="https://cdn.gramedia.com/uploads/items/9780593087633.jpg" alt="Buku 2" class="w-36 h-48 mx-auto" />
              <p class="text-lg font-semibold mt-4 text-neutral-600">The odds 1s out</p>
            </div>
          </a>
        </div>
        <!-- 3 -->
        <div class="w-1/4 mx-auto p-4 mt-4">
          <a href="#">
            <div class="bg-white shadow-lg p-4">
              <img src="https://cdn.gramedia.com/uploads/items/9786020633176_.Atomic_Habit.jpg" alt="Buku 2" class="w-36 h-48 mx-auto" />
              <p class="text-lg font-semibold mt-4 text-neutral-600">Atomic habits</p>
            </div>
          </a>
        </div>
        <!-- 4 -->
        <div class="w-1/4 mx-auto p-4 mt-4">
          <a href="#">
            <div class="bg-white shadow-lg p-4">
              <img src="https://cdn.gramedia.com/uploads/items/9786020628028_Seni-Berbicara-kepada-Siapa-Saja-Kapan-Saja-dan-di-Mana-Saja-ed.-Revisi.jpg" alt="Buku 2" class="w-36 h-48 mx-auto" />
              <p class="text-lg font-semibold mt-4 text-neutral-600">Seni Berbicara</p>
            </div>
          </a>
        </div>
        <!-- 5 -->
        <div class="w-1/4 mx-auto p-4 mt-4">
          <a href="#">
            <div class="bg-white shadow-lg p-4">
              <img src="https://cdn.gramedia.com/uploads/picture_meta/2023/6/8/j5hasrfmmczwjf35ccfe2x.jpg" alt="Buku 2" class="w-36 h-48 mx-auto" />
              <p class="text-lg font-semibold mt-4 text-neutral-600">Senja di alaska</p>
            </div>
          </a>
        </div>
        <!-- 6 -->
        <div class="w-1/4 mx-auto p-4 mt-4">
          <a href="#">
            <div class="bg-white shadow-lg p-4">
              <img src="https://cdn.gramedia.com/uploads/items/psychology_of_money.jpg" alt="Buku 2" class="w-36 h-48 mx-auto" />
              <p class="text-lg font-semibold mt-4 text-neutral-600">Money Psychology</p>
            </div>
          </a>
        </div>
      </div>

      <!-- kodingan untuk fitur lihat semua-->
    
    </main>
```

5. lanjut karena di website ini ada fitur lihat semua buku maka semua daftar buku akan muncul. simpan kodingan ini di kodingan 
```js
<main></main>
```
simpan di dalam sana di paling terakhir ada komentar kodingan untuk fitur lihat semua, kamu bisa tambahkan disana

```js
  <div id="lihatsemua" style="display: none">
        <div class="flex px-28">
          <!-- 1 -->
          <div class="w-1/4 mx-auto p-4 mt-4">
            <a href="#">
              <div class="bg-white shadow-lg p-4">
                <img src="https://cdn.gramedia.com/uploads/items/9786024553920-Bicara_itu_ada_seninya.jpg" alt="Buku 2" class="w-36 h-48 mx-auto" />
                <p class="text-lg font-semibold mt-4 text-neutral-600">bicara itu ada seninya</p>
              </div>
            </a>
          </div>
          <!-- 2 -->
          <div class="w-1/4 mx-auto p-4 mt-4">
            <a href="#">
              <div class="bg-white shadow-lg p-4">
                <img src="https://cdn.gramedia.com/uploads/picture_meta/2023/7/18/r6nezrwzruebpygb3couzq.jpg" alt="Buku 2" class="w-36 h-48 mx-auto" />
                <p class="text-lg font-semibold mt-4 text-neutral-600">Tone piece</p>
              </div>
            </a>
          </div>
          <!-- 3 -->
          <div class="w-1/4 mx-auto p-4 mt-4">
            <a href="#">
              <div class="bg-white shadow-lg p-4">
                <img src="https://cdn.gramedia.com/uploads/items/img20220101_11444970.jpg" alt="Buku 2" class="w-36 h-48 mx-auto" />
                <p class="text-lg font-semibold mt-4 text-neutral-600">Filosifi teras</p>
              </div>
            </a>
          </div>
          <!-- 4 -->
          <div class="w-1/4 mx-auto p-4 mt-4">
            <a href="#">
              <div class="bg-white shadow-lg p-4">
                <img src="https://cdn.gramedia.com/uploads/items/seni-negosiasi-_secrets-of-power-negotiating_-seni-canggih-untuk-melejitkan-kesuksesan-anda.jpg" alt="Buku 2" class="w-36 h-48 mx-auto" />
                <p class="text-lg font-semibold mt-4 text-neutral-600">Seni negosiasi</p>
              </div>
            </a>
          </div>
          <!-- 5 -->
          <div class="w-1/4 mx-auto p-4 mt-4">
            <a href="#">
              <div class="bg-white shadow-lg p-4">
                <img src="https://cdn.gramedia.com/uploads/picture_meta/2023/9/4/eqabs5dgzrpwkp7trvqajz.jpg" alt="Buku 2" class="w-36 h-48 mx-auto" />
                <p class="text-lg font-semibold mt-4 text-neutral-600">Jujutsu kaisen</p>
              </div>
            </a>
          </div>
          <!-- 6 -->
          <div class="w-1/4 mx-auto p-4 mt-4">
            <a href="#">
              <div class="bg-white shadow-lg p-4">
                <img src="https://cdn.gramedia.com/uploads/picture_meta/2023/10/10/6fdwgqqcfyo9ggpf9x9acg.jpg" alt="Buku 2" class="w-36 h-48 mx-auto" />
                <p class="text-lg font-semibold mt-4 text-neutral-600">Kaguya sama</p>
              </div>
            </a>
          </div>
        </div>
      </div>
```


6. lanjut kita akan membuat footer. simpan kodingan ini setelah  **main**
 ```js
  <footer class="h-52 mt-14 border static w-full bottom-0 py-28">
      <p class="text-center">@iqbal</p>
    </footer>
```

## fitur lihat semua buku menggunakan js

7. buat file js dengan nama perpus.js dan masukan kode berikut
 ```js
         function lainnya() {
        document.getElementById("lihatsemua").style.display = "block";
      }

      function info() {
        alert("halaman sedang di di kembangkan");
      }
 ```

 8. lanjut kita akan menghubungkan kodingan js ini ke html yang sudah di buat. simpan sebelum penutup body html
```js
<script src="perpus.js"></script>
```

## Asset 

berikut gambar yang ada di web yang saya buat

1.  <img src="img/logo.jpg" alt="logo" class="w-14 cursor-pointer" />
   
   ## note!
2. untuk gambar buku kamu bisa buka website [Gramedia](https://www.gramedia.com/) lalu kamu bisa cari buku yang ingin kamu tampilkan lalu 
   - kamu klik kanan poto
   - copy image address
   - lalu kamu pastekan di dalam **src img**
    ```js 
    <img src="masukan link disini" />
     ```
   
