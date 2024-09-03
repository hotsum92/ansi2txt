
```bash
echo -e "\e[38;5;31m RED \e[m"
```

## Terminal Colors

```bash
for ((i = 0; i < 16; i++)); do
    for ((j = 0; j < 16; j++)); do
        hex=$(($i*16 + $j))
        printf '\e[38;5;%dm0x%02X\e[m ' $hex $hex
    done
    echo "";
done
```

## Background Colors

```bash
for ((i = 0; i < 16; i++)); do
    for ((j = 0; j < 16; j++)); do
        hex=$(($i*16 + $j))
        printf '\e[48;5;%dm0x%02X\e[m ' $hex $hex
    done
    echo "";
done
```
