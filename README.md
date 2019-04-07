# Meu Pacote

Exemplo de um curso de Composer

## Exemplo de utilização

use Monolog\Logger;
use Monolog\Handler\StreamHandler;
use joantoniopn\CursoSON\Ola;

$log = new Logger('name');
$log->pushHandler(new StreamHandler('app.log', Logger::WARNING));

$log->warning((new Ola)->mensagem('Joao'));
$log->error('Bar');