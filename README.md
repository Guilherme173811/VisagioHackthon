# VisagioHackthon
Hackthon2020

Executar o arquivo front.py na pasta prototipo após descompactar-la.

Instalar todas as bibliotecas utilizadas no modelo.

import tensorflow as tf
from tensorflow.keras.preprocessing.text import Tokenizer
from tensorflow.keras.preprocessing.text import tokenizer_from_json
import re
import numpy as np
import json
import os 
import time
from selenium import webdriver
import dash
from dash.dependencies import Input, Output, State
import dash_html_components as html
import dash_core_components as dcc
import dash_bootstrap_components as dbc
