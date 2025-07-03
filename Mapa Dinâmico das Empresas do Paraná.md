# Mapa Dinâmico das Empresas do Paraná

## Descrição
Este projeto consiste em um mapa dinâmico e inteligente do estado do Paraná, focando nas sub-regiões 11, 12, 13, 14, 15, 16, 17, 18, 19, 21 e 22. O mapa exibe informações das maiores empresas de cada município ao passar o mouse sobre as regiões.

## Funcionalidades
- **Mapa Interativo**: Visualização geográfica dos municípios do Paraná com cores diferenciadas por região
- **Popup Dinâmico**: Ao clicar em um município, aparece um popup com informações detalhadas das empresas locais
- **Sidebar Informativa**: Painel lateral que exibe estatísticas em tempo real ao passar o mouse sobre os municípios
- **Dados Empresariais**: Informações de receita líquida, lucro líquido, rentabilidade e capital de giro
- **Design Responsivo**: Interface adaptável para desktop e dispositivos móveis

## Dados Utilizados
- **Fonte dos Dados Empresariais**: 500 maiores empresas do Paraná e Santa Catarina
- **Dados Geográficos**: GeoJSON dos municípios do Paraná (fonte: IBGE via GitHub)
- **Regiões Contempladas**: Sub-regiões 11-19, 21-22 conforme especificação

## Tecnologias
- **Frontend**: HTML5, CSS3, JavaScript
- **Biblioteca de Mapas**: Leaflet.js
- **Dados**: CSV (empresas) + GeoJSON (geografia)
- **Servidor**: Python HTTP Server (para desenvolvimento)

## Como Utilizar

### 1. Abrir o Mapa
- Abra o arquivo `index.html` em qualquer navegador web moderno
- O mapa carregará automaticamente os dados das empresas e a geografia do Paraná

### 2. Interagir com o Mapa
- **Visualizar Informações**: Passe o mouse sobre qualquer município para ver as informações na sidebar
- **Ver Detalhes**: Clique em um município para abrir um popup com dados detalhados das empresas
- **Navegar**: Use os controles de zoom (+/-) para aproximar ou afastar a visualização

### 3. Interpretar as Cores
- **Verde**: Alta concentração de empresas (5+ empresas)
- **Laranja**: Média concentração (2-4 empresas)
- **Vermelho**: Baixa concentração (1 empresa)
- **Cinza**: Sem dados de empresas

## Estrutura dos Arquivos
```
mapa_parana/
├── index.html                      # Página principal
├── script.js                       # Lógica do mapa e interações
├── parana_empresas_com_regiao.csv   # Dados das empresas
└── parana_municipios.geojson        # Dados geográficos
```

## Informações Técnicas

### Dados das Empresas
O arquivo CSV contém as seguintes colunas:
- **Cidade**: Nome do município
- **Receita Líq.**: Receita líquida da empresa
- **Lucro Líquido**: Lucro líquido da empresa
- **Rentabilidade Receita**: Percentual de rentabilidade
- **Capital de Giro**: Capital de giro da empresa
- **Sub-região**: Região à qual o município pertence

### Mapeamento de Regiões
- **Região 11 (Campo Mourão)**: 29 municípios
- **Região 12 (Umuarama)**: 17 municípios
- **Região 13 (Cianorte)**: 12 municípios
- **Região 14 (Paranavaí)**: 25 municípios
- **Região 15 (Maringá)**: 22 municípios
- **Região 16 (Apucarana)**: 13 municípios
- **Região 17 (Londrina)**: 11 municípios
- **Região 18 (Cornélio Procópio)**: 14 municípios
- **Região 19 (Jacarezinho)**: 20 municípios
- **Região 21 (Telêmaco Borba)**: 8 municípios
- **Região 22 (Ivaiporã)**: 14 municípios

## Características do Design
- **Interface Moderna**: Design com gradientes e efeitos visuais
- **Cores Regionais**: Cada região possui uma cor específica para fácil identificação
- **Animações Suaves**: Transições e hover effects para melhor experiência do usuário
- **Tipografia Legível**: Fontes modernas e hierarquia visual clara

## Requisitos do Sistema
- Navegador web moderno (Chrome, Firefox, Safari, Edge)
- Conexão com internet (para carregar as bibliotecas Leaflet.js)
- JavaScript habilitado

## Observações
- O mapa foca apenas nas regiões especificadas (11-19, 21-22)
- Municípios fora dessas regiões aparecem transparentes
- Os dados são baseados no arquivo fornecido das 500 maiores empresas
- A ferramenta é ideal para análise de mercado e planejamento comercial

