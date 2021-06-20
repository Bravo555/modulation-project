# modulation-project

## Getting started

Create a python virtual environment and install the dependencies:

```sh
$ python -m venv .venv
$ source .venv/bin/activate
$ pip install -r requirements.txt
```

Next, prepare a config file:

```
; *modulation* *input_size* *signal_to_noise_ratio* *orders* *amplitudes*
ASK 12000 0.1 4 1.0
PSK 12000 0.1 4 1.0
APSK 12000 0.1 4,4 1.0,2.0

ASK 12000 0.2 4 1.0
PSK 12000 0.2 4 1.0
APSK 12000 0.2 4,4 1.0,2.0

...
```

To run the modulation simulation with the included config file `config.ini`:

```sh
$ python src/main.py config.ini
```
