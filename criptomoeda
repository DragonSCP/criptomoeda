import requests
import time

# Dados do pool de mineração
POOL_URL = 'pool.exemplo.com:3333'
WALLET_ADDRESS = '45Ak7U2bMdxdbNDKjgYuAxCLx4119YBLu8tUbFLF1GKmQT9CJTXPTWdHt8n56WrZimC82TqPjGiHNKT7SdNLZxHV8WjG2Q7'

# Função para minerar
def mine():
    while True:
        # Conectar ao pool e iniciar mineração
        response = requests.post(f'http://{POOL_URL}/start', data={'address': WALLET_ADDRESS})
        if response.status_code == 200:
            print('Minerando...')
        else:
            print('Erro ao conectar ao pool.')
        time.sleep(60)  # Esperar 1 minuto antes de verificar novamente

if __name__ == '__main__':
    mine()
