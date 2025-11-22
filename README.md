# 🏥 Sistema de Gerenciamento de Saúde  
Um sistema de gerenciamento de pacientes e médicos desenvolvido em **Python**, utilizando **Programação Orientada a Objetos (POO)**, com filas de atendimento **preferencial** e **convencional** para diferentes especialidades médicas.

---

## 🔧 Tecnologias utilizadas
- **Python 3**
- **POO (Classes e Objetos)**
- Estruturas de dados:
  - Listas
  - Dicionários
  - Filas (implementadas manualmente)

---

## 🎯 Objetivo do projeto
O objetivo deste sistema é simular o funcionamento de uma clínica/hospital, permitindo:

- Cadastro de médicos  
- Alteração e remoção de médicos  
- Cadastro de pacientes  
- Gerenciamento de filas por especialidade  
- Atendimento com prioridade para **IDOSO**, **PCD** e **GESTANTE**  
- Separação entre fila **preferencial** e **convencional**  
- Chamada de pacientes conforme ordem de chegada (FIFO)

---

## 📁 Estrutura do projeto
/
│── classes/
│ ├── doctor.py # Classe Doctor
│ ├── patient.py # Classe Patient
│ └── queue.py # Implementação de Fila
│
└── main.py # Arquivo principal com menu e operações

---

## 👨‍⚕️ Classes principais

### **Doctor**
Representa um médico, contendo:
- nome  
- especialidade  

### **Patient**
Representa um paciente, contendo:
- nome  
- tipo (Idoso, PCD, Gestante ou Paciente)  
- especialidade desejada  

### **Queue**
Implementa uma fila com:
- `enqueue()`  
- `dequeue()`  
- `isEmpty()`  
- `__str__()` para exibir a fila

---

## 🔥 Funcionalidades implementadas

### ✔️ 1. Gerenciamento de Médicos
- Cadastrar médico  
- Alterar nome ou especialidade  
- Excluir médico  
- Listar médicos  

---

### ✔️ 2. Gerenciamento de Pacientes
- Cadastrar paciente  
- Enviar para fila preferencial (idoso, PCD, gestante)  
- Enviar para fila convencional  

---

### ✔️ 3. Filas por Especialidade

#### 🟦 Preferencial  
Especialidades:
- clínico geral  
- pediatria  
- ortopedia  
- geriatria  

#### 🟩 Convencional  
Mesmas especialidades, mas separadas.

---

### ✔️ 4. Chamada de Paciente
Fluxo de chamada:
1. Preferencial  
2. Convencional  
3. Caso as duas vazias → mensagem “Fila vazia”

---
