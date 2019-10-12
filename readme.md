# Orleans Demo

Este � um exemplo de uso do framework Orleans da Microsoft para a constru��o de aplica��es escal�veis e resilientes.
A ideia aqui � simular um sistema que gerencia dispositivos que medem a temperatura (IoT). Cada um dos dispositivos envia para uma API a sua temperatura atual, que � armazenada nos atores (grains) hospedados na camada intermedi�ria (stateful).

![Alt text](docs/architecture.png)

Este exemplo considera a persist�ncia dos atores e a gest�o do cluster com o uso de um banco de dados SQL Server. A URL de conex�o deve ser configurada como um secret da aplica��o (chaves *ClusterStorage* e *GrainStorage*)

O exemplo foi desenvolvido em uma m�quina Ubuntu, com .NET Core 2.2 e rodando um SQL Server 2019 como um container (Docker).