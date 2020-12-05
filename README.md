# Решения заданий лабораторной работы по DHCP(Компьютерные сети)

## Описать этапы резервации IP адреса клиентом у DHCP сервера
### Указать IP источника и назначения на каждом этапе

1. Запрос на обнаружение DHCP сервера: хост отправляет запрос в широковещательный канал для обнаружения DHCP сервера.
```
scr IP: 0.0.0.0
dst IP: 255.255.255.255
```
![Discover request](https://github.com/mihai-valentin/computer_networks_dhcp/blob/main/discover.png)

2. Отправка предложения от DHCP сервера: сервер отвечает на запрос клиента предложением с настройками.
```
src IP: 178.168.0.1
dst IP: 255.255.255.255
```
![Offer request](https://github.com/mihai-valentin/computer_networks_dhcp/blob/main/offer.png)

3. Ответный запрос на предложение DHCP сервера: клиент выбирает DHCP сервер и отправляет запрос серверу.
```
src IP: 0.0.0.0
dst IP: 255.255.255.255
```
![Request](https://github.com/mihai-valentin/computer_networks_dhcp/blob/main/request.png)

4. Подтверждение получения ответа на запрос. Применение настроек.
```
src IP: 178.168.0.1
dst IP: 255.255.255.255
```
![Pack request](https://github.com/mihai-valentin/computer_networks_dhcp/blob/main/pack.png)

## Построить схему в Packet Tracer

[Макет сети](https://github.com/mihai-valentin/computer_networks_dhcp/blob/main/dhcp.pkt)

## Настроить DHCP server в Windows

## Настроить DHCP server в Linux
