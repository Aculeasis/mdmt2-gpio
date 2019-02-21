# Опытный образец плагина для  [mdmTerminal2](https://github.com/Aculeasis/mdmTerminal2)

# Установка
```
# для плат на процессорах H2+ и H3
cd ~
git clone https://github.com/duxingkei33/orangepi_PC_gpio_pyH3
cd orangepi_PC_gpio_pyH3
~/mdmTerminal2/env/bin/python -m setup.py install
cd ~/mdmTerminal2/src/plugins
git clone https://github.com/Flokss/mdmt2-gpio


# для плат на процессорах H5
cd ~
git clone https://github.com/herzig/orangepi_PC_gpio_pyH5
cd orangepi_PC_gpio_pyH5
~/mdmTerminal2/env/bin/python -m setup.py install
cd ~/mdmTerminal2/src/plugins
git clone https://github.com/Flokss/mdmt2-gpio

```
И перезапустить терминал.
# Описание
Плагин управляет светодиодами подключенными к gpio PA11 и PA12 (проверено на платах с процессорами H2+ и H3, возможно будет работать и с H5)
```
 PA12 включает светодиод при проговаривании текста терминалом
 PA11 включает светодиод при записи голоса
```
# Настройка
Настройки хранятся в mdmTerminal2/src/data/gpio_config_config.json, файл будет создан при первом запуске:

led_on: логический уровень включенного светодиода 0 или 1, по умолчанию 1

