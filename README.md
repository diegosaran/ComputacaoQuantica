# Demonstrando o Chute de Fase (Phase Kickback) com Qiskit

## 🎯 Objetivo
Demonstrar o fenômeno do chute de fase em um circuito quântico simples de dois qubits, utilizando o Qiskit, e mostrar como uma rotação de fase aplicada ao qubit alvo afeta o qubit de controle.

## 📚 Contexto Teórico
Na computação quântica, quando o qubit de controle está em superposição e uma porta controlada (`CRZ(θ)`) é aplicada, a fase aplicada ao alvo pode "refletir" de volta para o controle. Isso evidencia a natureza unitária e reversível das operações quânticas — algo que não ocorre na computação clássica.

## 🧪 Etapas do Experimento

1. Inicializar um circuito quântico de 2 qubits.
2. Aplicar `H` no qubit de controle e `X` no alvo (para colocá-lo em |1⟩).
3. Aplicar `CRZ(θ)` — a fase afeta o alvo se o controle for |1⟩.
4. Aplicar um `H` final no controle — converte a fase em diferença de probabilidade.
5. Visualizar o statevector e as esferas de Bloch.
6. Simular e medir os resultados com o `AerSimulator`.

## 🧠 Importância do Fenômeno
O chute de fase é um componente essencial em:
- Estimativa de Fase Quântica (QPE)
- Algoritmo de Shor
- Simulações quânticas

## 📊 Visualizações
- Amplitudes do statevector
- Representações na esfera de Bloch
- Histogramas de medição (com e sem Hadamard final)

## 📎 Informações Adicionais
- Criado por: Diego Saran
- Licença: MIT
- Versão: 1.0
- Data: Julho de 2025

## 🧰 Requisitos
- Qiskit >= 2.1.0
- Qiskit IBM Runtime >= 0.40.0
