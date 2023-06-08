# ransomware-python
CyberSecurity


## Criptografar e descriptografar um arquivo usando AES em modo CTR

Este código em Python demonstra como criptografar e descriptografar um arquivo usando o algoritmo AES em modo CTR. O código utiliza a biblioteca `pyaes` para realizar a criptografia e descriptografia dos dados.

### Passos do processo de criptografia:

1. Importar os módulos necessários:
   - `os`: fornece funções para interagir com o sistema operacional.
   - `pyaes`: biblioteca que implementa o algoritmo de criptografia AES.

2. Especificar o nome do arquivo a ser criptografado:
   - Neste exemplo, o nome do arquivo é definido como "teste.txt.ransomwaretroll". Certifique-se de substituir pelo nome do arquivo que você deseja criptografar.

3. Abrir o arquivo em modo de leitura binária:
   - O arquivo é aberto usando a função `open` com o modo "rb" para leitura binária.
   - Os dados do arquivo são lidos e armazenados na variável `file_data`.
   - Em seguida, o arquivo é fechado usando o método `close`.

4. Definir a chave de criptografia:
   - A chave de criptografia é definida como um objeto de bytes (`bytes`).
   - Neste exemplo, a chave é definida como "testeransomwares". Você pode modificar a chave conforme necessário para sua aplicação.

5. Criar uma instância do objeto AES em modo CTR:
   - A biblioteca `pyaes` é usada para criar um objeto AES em modo CTR, passando a chave como parâmetro.
   - O objeto AES será usado para criptografar e descriptografar os dados do arquivo.

6. Criptografar os dados do arquivo:
   - Os dados do arquivo são criptografados chamando o método `encrypt` do objeto AES, passando os dados do arquivo como parâmetro.
   - Os dados criptografados são armazenados na variável `crypto_data`.

7. Remover o arquivo original criptografado:
   - O arquivo original criptografado é removido usando a função `os.remove(file_name)`.
   - Tenha cuidado ao usar essa operação, pois a remoção do arquivo é irreversível.

8. Criar um novo arquivo para armazenar os dados criptografados:
   - O nome do novo arquivo é definido como "teste.txt".
   - Um novo arquivo é criado usando a função `open` com o modo "wb" para escrita binária.
   - Os dados criptografados são gravados no novo arquivo usando o método `write`.
   - Por fim, o novo arquivo é fechado usando o método `close`.

### Passos do processo de descriptografia:

1. Importar os módulos necessários:
   - `os`: fornece funções para interagir com o sistema operacional.
   - `pyaes`: biblioteca que implementa o algoritmo de criptografia AES.

2. Especificar o nome do arquivo a ser descriptografado:
   - Neste exemplo, o nome do arquivo é definido como "teste.txt".
   - Certifique-se de substituir pelo nome do arquivo criptografado que você deseja descriptografar.

3. Abrir o arquivo em modo de leitura binária:
   - O arquivo é aberto usando a função `open` com o modo "rb" para leitura binária.
   - Os dados do arquivo criptografado são lidos e armazenados na variável `file_data`.
   - Em seguida, o arquivo é fechado usando o método `close`.

4. Definir a chave de descriptografia:
   - A chave de descriptografia é a mesma chave usada na criptografia.
   - Certifique-se de usar a mesma chave que foi usada para criptografar o arquivo.

5. Criar uma instância do objeto AES em modo CTR:
   - A biblioteca `pyaes` é usada para criar um objeto AES em modo CTR, passando a chave como parâmetro.
   - O objeto AES será usado para criptografar e descriptografar os dados do arquivo.

6. Descriptografar os dados do arquivo:
   - Os dados do arquivo são descriptografados chamando o método `decrypt` do objeto AES, passando os dados do arquivo como parâmetro.
   - Os dados descriptografados são armazenados na variável `decrypt_data`.

7. Remover o arquivo original criptografado:
   - O arquivo original criptografado é removido usando a função `os.remove(file_name)`.
   - Tenha cuidado ao usar essa operação, pois a remoção do arquivo é irreversível.

8. Criar um novo arquivo para armazenar os dados descriptografados:
   - O nome do novo arquivo é definido como "teste.txt".
   - Um novo arquivo é criado usando a função `open` com o modo "wb" para escrita binária.
   - Os dados descriptografados são gravados no novo arquivo usando o método `write`.
   - Por fim, o novo arquivo é fechado usando o método `close`.

### Observações:
- Este código é fornecido apenas como exemplo e não deve ser usado para fins maliciosos.
- Lembre-se de ter cuidado ao lidar com operações de remoção de arquivos, pois elas podem resultar na perda permanente de dados.
- Certifique-se de ter instalado o pacote `pyaes` antes de executar este código.



