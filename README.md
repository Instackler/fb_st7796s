# Краткое руководство по установке

## long story short

```console
cd ~ 
rm -r fb_st7796s
git clone https://github.com/evgs/fb_st7796s.git
fb_st7796s/install.sh
```
Если дисплей повёрнут горизонтально, то дополнительно запустить скрипт
```console
fb_st7796s/switch_to_landscape.sh
```

# Драйвер для экрана MKS TS35 V2.0

Соединение экрана с разъёмом GPIO Orange Pi3 LTS осуществляется в соответствии с таблицей

| Дисплей | Функция   | GPIO | пин | Комментарий                            |
|---------|-----------|------|-----|----------------------------------------|
| EXP1_1  | BEEPER    | PD21 | 22  | Управление пищалкой                    |
| EXP1_3  | LED_BKL   | PD18 | 12  | Подсветка дисплея                      |
| EXP1_4  | RST       | nc   | nc  | Сброс TFT-дисплея                      |
| EXP1_5  | TOUCH_CS  | PH03 | 24  | Выборка шины тачскрина                 |
| EXP1_6  | TOUCH_IRQ | PL10 | 15  | Запрос прерывания тачскрина по касанию |
| EXP1_7  | TFT_CS    | PL08 | 26  | Выборка шины TFT                       |
| EXP1_8  | D/C       | PD15 | 16  | Выборка данных/команд на шине TFT      |
| EXP1_9  | GND       | GND  | 09  | Общий (питание)                        |
| EXP1_10 | +5V       | +5V  | 02  | Питание дисплея                        |
| EXP2_1  | MISO      | PH06 | 21  | Линия MISO шины SPI                    |
| EXP2_2  | CLK       | PH04 | 23  | Линия SCK шины SPI                     |
| EXP2_6  | MOSI      | PH05 | 19  | Линия MISO шины SPI                    |
| EXP2_9  | GND       | GND  | 25  | Общий (сигнальный)                     |

Драйвер для экрана на контроллере st7796. [Описание установки и настройки](https://sergey1560.github.io/fb4s_howto/mks_ts35/)
