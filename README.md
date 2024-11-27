# prime_energy_brasil

Documentação do Projeto: Prime Energy Brasil
Obejetivo
O projeto Prime Energy Brasil foi idealizado como uma solução mobile para enfrentar os desafios climáticos e energéticos, promovendo eficiência no uso da energia elétrica em residências e pequenas empresas. Com eventos climáticos extremos cada vez mais frequentes e a necessidade de redução das emissões de gases de efeito estufa, o monitoramento e a otimização do consumo energético se tornaram indispensáveis.
Este aplicativo oferece um meio intuitivo e eficiente para os usuários acompanharem em tempo real o consumo energético, identificarem desperdícios e ajustarem o uso de aparelhos elétricos, contribuindo para a sustentabilidade e redução de custos.
________________


Arquitetura da Solução
O projeto foi desenvolvido utilizando uma arquitetura baseada em microsserviços, com os seguintes componentes principais:
1. Frontend: Aplicativo desenvolvido em React Native utilizando Expo para maior agilidade no desenvolvimento e compatibilidade entre plataformas (iOS e Android).
2. Backend: Gerenciado com Firebase, responsável pelo banco de dados em tempo real e autenticação de usuários.
3. Camada de Visualização: Uso do componente React Native Speedometer Chart para exibir os dados de consumo energético em um painel intuitivo.
4. Gerenciamento de Dados: Cloud Firestore para armazenamento e atualização dos dados energéticos.
5. Integração com Serviços Externos: APIs para configurar dispositivos inteligentes, se aplicável.
________________


Ferramentas e Tecnologias
* Linguagem de Desenvolvimento: React Native
* Plataforma de Desenvolvimento: Expo.io
* Backend: Firebase (Autenticação e Banco de Dados)
* Componentes UI/UX: NativeBase e React Native Navigation
* Visualização de Dados: React Native Speedometer Chart
________________


Funcionalidades
1. Monitoramento de Consumo Energético em Tempo Real
   * O aplicativo exibe o consumo energético em três fases (L1, L2, L3) utilizando gráficos de velocidade intuitivos.
   * Atualizações são sincronizadas automaticamente com o banco de dados em tempo real.
2. Relatórios de Consumo Personalizados
   * Geração de relatórios diários e mensais sobre o consumo energético.
   * Sugestões de economia baseadas em padrões de uso identificados.
________________


Prototipação Não Funcional (Mockup)
Os mockups foram desenvolvidos para demonstrar a interface amigável e funcionalidade básica do aplicativo:
1. Tela Inicial: Exibe as fases (L1, L2, L3) em gráficos de velocidade.
2. Relatórios: Acesso rápido aos relatórios de consumo com sugestões para redução de gastos.
________________


Gerenciamento de Memória
O gerenciamento de memória foi otimizado utilizando as seguintes práticas:
* Uso de bibliotecas leves e otimizadas para gráficos e navegação.
* Evitar re-renderizações desnecessárias com técnicas como memoização e hooks do React (ex.: useMemo e useCallback).
* Armazenamento local mínimo, apenas para dados temporários, utilizando o AsyncStorage para persistência.
* Realização de chamadas assíncronas ao banco de dados para evitar bloqueio na interface do usuário.
________________


Interface com o Usuário
O design do Prime Energy Brasil prioriza a simplicidade e a experiência do usuário:
* Interface Intuitiva: Navegação limpa e fácil acesso aos gráficos e relatórios.
* Painel Visual: Exibição clara e em tempo real dos dados, utilizando gráficos de velocidade que simulam um velocímetro para cada fase de energia.
* Design Responsivo: Compatibilidade total com diferentes tamanhos de tela (smartphones e tablets).
________________


Passo a Passo para Execução
Pré-requisitos
* Node.js instalado.
Expo CLI instalado globalmente:
bash
Copy code
npm install expo-cli --global
* * Conta configurada no Firebase seguindo este tutorial.
Instalação
Clone o repositório:
bash
Copy code
git clone https://github.com/joaoj1/prime_energy_brasil
cd prime-energy-brasil
1. Instale as dependências:
bash
Copy code
npm install
2. 3. Configure o arquivo APIchave.js com suas credenciais do Firebase.
Execução
Inicie o servidor de desenvolvimento:
bash
Copy code
expo start
1. 2. Escaneie o QR Code com o aplicativo Expo Go para rodar no dispositivo móvel.
________________


Aprendizados e Próximos Passos
Durante o desenvolvimento do Prime Energy Brasil, aprendemos a importância de integrar interfaces intuitivas com dados em tempo real para oferecer uma experiência diferenciada aos usuários.
Próximos passos:
* Integração com dispositivos IoT para automação de aparelhos.
* Expansão para monitoramento em outros setores (comercial e industrial).
