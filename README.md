# **Energize: Plataforma de Otimização e Monitoramento do Consumo de Energia**

## **Descrição do Projeto**
O **Energize** é uma solução inovadora que utiliza tecnologias modernas para:
- **Reduzir custos energéticos**
- **Minimizar desperdícios**
- **Promover práticas sustentáveis**

A plataforma combina sensores inteligentes, hubs de controle, inteligência artificial e um sistema intuitivo de visualização para otimizar o consumo de energia elétrica.

---

## **Solução Proposta**
### **Componentes da Solução**
1. **Sensores de Consumo de Energia**
   - **Descrição**: Dispositivo ESP32 com medidores de corrente conectados ao WiFi.
   - **Função**: Captura dados de consumo em tempo real para análise precisa.
   
2. **Hub de Controle**
   - **Descrição**: ESP32 centraliza os dados dos sensores.
   - **Função**: Envia dados para a API, garantindo conectividade e processamento local.

3. **Histórico e Relatórios**
   - **Descrição**: Desenvolvido em Java.
   - **Função**: Apresenta dados diários, semanais e mensais sobre o consumo.

4. **Dashboard Interativo**
   - **Descrição**: Interface visual e intuitiva.
   - **Funcionalidades**: Dados em tempo real, alertas, dicas de economia e informações sobre fontes renováveis.

5. **Banco de Dados**
   - **Função**: Armazena histórico de consumo e sugestões.
   - **Benefício**: Integridade e acesso fácil às informações.

---

## **Benefícios de Negócios**
1. **Redução de Custos**
   - Identificação de picos de consumo e horários ideais para uso.
   - Redução significativa dos gastos com energia elétrica.

2. **Sustentabilidade**
   - Incentivo ao uso eficiente da energia e fontes renováveis.
   - Redução da pegada de carbono.

3. **Decisões Baseadas em Dados**
   - Insights precisos para otimização do consumo.

4. **Aumento da Eficiência**
   - Monitoramento em tempo real e relatórios detalhados.

5. **Diferenciação de Mercado**
   - Empresas podem reforçar a imagem de responsabilidade ambiental.

---

## **Estrutura do Banco de Dados**
### **Tabelas Criadas**
- **`tb_alerta`**: Registra alertas emitidos.
- **`tb_consumo`**: Armazena dados de consumo energético.
- **`tb_dispositivo`**: Contém informações sobre dispositivos.
- **`tb_sugestao`**: Sugestões para economia de energia.
- **`tb_usuario`**: Dados dos usuários do sistema.
- **`tb_auditoria`**: Log de operações realizadas no banco.

### **Relacionamentos**
As tabelas utilizam chaves estrangeiras para garantir integridade referencial.

---

## **Inserção e Manipulação de Dados**
### **Procedures de Inserção**
- **`sp_insert_tb_alerta`**: Inserir alertas.
- **`sp_insert_tb_consumo`**: Inserir dados de consumo.
- **`sp_insert_tb_dispositivo`**: Inserir dispositivos.
- **`sp_insert_tb_sugestao`**: Inserir sugestões.
- **`sp_insert_tb_usuario`**: Inserir usuários.

### **Funções**
- **`fn_calcular_custo_medio`**: Calcula o custo médio por kWh.
- **`fn_validar_email`**: Valida endereços de e-mail.

### **Triggers**
Os triggers auditam operações nas tabelas:
- **`trg_audit_tb_alerta`**, **`trg_audit_tb_consumo`**, **`trg_audit_tb_dispositivo`**, **`trg_audit_tb_sugestao`**, **`trg_audit_tb_usuario`**.

### **Exportação e Integração**
A procedure **`sp_exportar_json_mongodb`** exporta dados em JSON para integração com MongoDB.

---

## **Conclusão**
O banco de dados Energize é uma solução robusta, eficiente e escalável para monitoramento e análise energética, promovendo sustentabilidade e eficiência. 
