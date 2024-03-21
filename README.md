<div align="center">
	<h1>🗣️ minitalk</h1>
  <img src="https://i.redd.it/d1od5plmoeiz.jpg"/>
	<p>Bu proje, C'deki sinyaller kullanılarak uygulanan basit bir client-server iletişim sistemidir. Client, server'a bir mesaj gönderir ve server, mesajı karakter karakter alır ve görüntüler.</p>
   <br />
	<img src="https://img.shields.io/badge/norminette-passing-success"/>
	<a href="https://developer.apple.com/library/archive/documentation/Performance/Conceptual/ManagingMemory/Articles/FindingLeaks.html"><img src="https://img.shields.io/badge/leaks-none-success" /></a>
	<img src="https://img.shields.io/badge/-100%2F125-success?logo=42&logoColor=fff" />
</div>

## Usage

1. Repo'yu clone'layın:

```bash
git clone 
```

2. Makefile'ı kullanarak source kodu derleyin:
```bash
make
```

> 2 executable file oluşmaktadır: `client` ve `server`.

3. `server` binary dosyasını execute ederek server'ı başlatın:
```bash
./server
```

> Server'ın process id'si (PID) terminalde gözükür.

4. Ayrı bir terminal penceresinde, server'ın PID'si ve iletmek istediğiniz mesajla client binary file'ı çalıştırarak client'ı başlatın:

```bash
./client <server_pid> <message>
```

> `<server_pid>` kısmını server tarafından görüntülenen PID ile ve `<message>` kısmını göndermek istediğiniz metin ile değiştirin.

Example:
```bash
./client 1760 Trrrrum, trrrrum, trrrrum! Trak tiki tak! Makinalaşmak istiyorum!
```

> Bu, ilgili PID ile sunucuya ilgili mesajı gönderecektir.

5. Server, mesajı alacak ve terminalde gösterecektir:

```bash
Trrrrum, trrrrum, trrrrum! Trak tiki tak! Makinalaşmak istiyorum!
```

> Server her karakteri aldığında gösterecektir.

6. Server'a birden fazla mesaj göndermek için 4. ve 5. adımları tekrarlayabilirsiniz.


