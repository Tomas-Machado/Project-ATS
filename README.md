# Project-ATS
# SpotifUM Testing Audit - Tomás Machado (A104186)

Este projeto contém a auditoria de testes e análise de software do sistema SpotifUM.

## Pré-requisitos
- Java 11 ou 17
- Maven 3.8+

## Como Reproduzir os Resultados

### 1. Executar Testes Unitários e de Propriedade (JUnit 5 + jqwik)
```bash
mvn test
```

### 2. Gerar Relatório de Cobertura (JaCoCo)
```bash
mvn jacoco:report
```
# Relatório disponível em: target/site/jacoco/index.html

### 3. Executar Testes de Mutação (PIT)
```bash
mvn pitest:mutationCoverage
```
# Relatório disponível em: target/pit-reports/

## Nota sobre EvoSuite
Os testes do EvoSuite foram gerados num ambiente isolado (Java 8) para compatibilidade e encontram-se na pasta `evosuite_results` como evidência da auditoria técnica.
