
## Spis
* [Informacje](#Informacje)
* [Wymagania](#Wymagania)
* [Instalacja playbooka](#Instalacja)

## Informacjee
Playbook do instalacji xkasaneta na komputerze z ekranem niedotykowym w wersji 2.2.17. Instalowana wersja xkasnet-klient-notouch. Wczesniej musi być zainstalowany system operacyjny ubuntu 22.04.
Ewentualnie można zainstalować system z innego playbooka:

ansible-pull -i hosts -U http://github.com/netispl/wzorzec

Dotakowo dodawny jest user ansiblenet i vpn.

## Wymagania
Testowane na Ubuntu 22.04 64 bit desktop
https://cdimage.ubuntu.com/daily-live/current/jammy-desktop-amd64.iso

W celu odpalenia playbooka nalezy uruchomić:

```
 apt-add-repository --yes --update ppa:ansible/ansible
 apt-get install git ansible --yes --force-yes
```

## Instalacja playbooka
Instalacja projektu (wymaga podania hasła do odszyfrowania klucza):

```
 ansible-pull --vault-id @prompt -i hosts -U http://github.com/netispl/xkasnet-notouch-ubuntu22
```


