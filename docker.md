<aside>
** Docker makes development efficient and predictable. **

</aside>

`Docker` 是一個開發、交付和運行應用程式的開源平台，它所提供的容器擁有鬆散隔離的環境，負責封裝和運行應用程式。

正因為容器將運行應用程式所需要的一切都封裝在一起，讓你可以不用去思考現在執行在哪個主機上，可以非常簡單、快速地轉移你的專案，不用擔心環境的問題。

# Docker 底層技術

`Docker` 是由Go 語言撰寫而成，並有幾個功能是使用Linux 核心來完成的。

- `Namespace` : 用來隔離不同容器的執行空間。
- `Cgroup` : 用來分配硬體資源。
- `AUFS ( chroot )` : 用來建立不同容器的檔案系統。
- `SELinux` : 用來確保容器的網路安全。
- `Netlink` : 讓不同容器之間的行程可以進行溝通。
- `Netfilter` : 建立容器埠為基礎的網路防火牆封包過濾。
- `AppArmor` : 保護容器的網路及執行安全。
- `Linux Bridge` : 讓不同的容器或不同主機上的容器之間能進行溝通。
