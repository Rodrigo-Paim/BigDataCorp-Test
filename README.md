# BigDataCorp-Test

Front-end do site: O front-end será responsável por exibir a interface do site para os usuários. Ele deve permitir que os usuários criem contas, façam login e naveguem pelas opções de ingressos disponíveis.

Back-end do site: O back-end do site será responsável pelo processamento das solicitações do front-end, autenticação de usuários e gerenciamento do estoque de ingressos. Ele deve ser projetado para lidar com uma grande carga de tráfego, uma vez que o site é extremamente concorrido.

Banco de dados: Um banco de dados deve ser utilizado para armazenar informações sobre os usuários registrados, detalhes da compra de ingressos e informações de estoque. Ele deve ser escalável e ter uma capacidade adequada para armazenar um grande número de registros.

Sistema de autenticação: Para garantir que apenas usuários autenticados possam finalizar a compra de ingressos, é necessário implementar um sistema de autenticação seguro. Isso pode ser feito por meio de tokens de acesso, como JWT (JSON Web Tokens), que são emitidos para usuários após a autenticação bem-sucedida e são verificados em cada solicitação subsequente.

Controle de estoque em tempo real: Para evitar que um usuário compre um ingresso que já foi vendido, é necessário implementar um sistema de controle de estoque em tempo real. Isso pode ser feito usando um mecanismo de bloqueio do estoque assim que um usuário iniciar o processo de compra. Se a compra não for concluída em um determinado período de tempo, o ingresso será liberado novamente.

Serviço de fila: Dado que o número de ingressos é limitado e o número de acessos é alto, um serviço de fila pode ser implementado para gerenciar o processo de compra de ingressos. Isso garantirá que as solicitações de compra sejam processadas na ordem em que foram recebidas, evitando que uma pessoa com uma conexão mais rápida passe à frente de uma pessoa com uma conexão mais lenta.
