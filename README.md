# OBFUSCATOR

Dùng để làm rối code Python đơn giản.

## Yêu cầu

- Python 3.12

## Cài đặt & chạy

```bash
git clone https://github.com/raphaelkissu/obfuscator.git
cd obfuscator
python main.py
```

## Cách dùng

```bash
python main.py
```

Sau đó nhập:

```
File đầu vào  : <example.py>
File đầu ra   : <example_obf.py>
```

Mỗi lần chạy sẽ cho output khác nhau

Demo :
INPUT
```python
print('hello, world!')
```
OUTPUT
```python
import marshal,base64,zlib

Δ482=lambda λ193:marshal.loads(__import__('zlib').decompress(__import__('base64').b64decode(λ193)))
Ω731=lambda x:exec(Δ482(x))

Ω731('eJxLyslMUbJS8nMz1FHKTS3JzM8DAK8EBVY=')
```
