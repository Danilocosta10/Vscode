# VscodePular para o conteúdo
Menu de navegação
atv10

Código
Problemas
atv10
/LEIA-ME.md
94 linhas (76 loc) · 3,45 KB

Visualização

Código

Culpa
atv10
class Atividade { private String nome; private int duração; // duração em minutos private String dificuldade;

public String getNome() { return nome; }
public void setNome(String nome) { this.nome = nome; }

public int getDuracao() { return duracao; }
public void setDuracao(int duracao) { this.duracao = duracao; }

public String getDificuldade() { return dificuldade; }
public void setDificuldade(String dificuldade) { this.dificuldade = dificuldade; }
}

class Pedalar estende Atividade { private String tipoBicicleta; private booleano usaCapacete;

public String getTipoBicicleta() { return tipoBicicleta; }
public void setTipoBicicleta(String tipoBicicleta) { this.tipoBicicleta = tipoBicicleta; }

public boolean isUsaCapacete() { return usaCapacete; }
public void setUsaCapacete(boolean usaCapacete) { this.usaCapacete = usaCapacete; }
}

class ArtesMarciais estende Atividade { private String estilo; faixa de String privada;

public String getEstilo() { return estilo; }
public void setEstilo(String estilo) { this.estilo = estilo; }

public String getFaixa() { return faixa; }
public void setFaixa(String faixa) { this.faixa = faixa; }
}

class Danca estende Atividade { private String estiloDanca; privado em anosPrática;

public String getEstiloDanca() { return estiloDanca; }
public void setEstiloDanca(String estiloDanca) { this.estiloDanca = estiloDanca; }

public int getAnosPratica() { return anosPratica; }
public void setAnosPratica(int anosPratica) { this.anosPratica = anosPratica; }
}

public class Main { public static void main(String[] args) { Pedalar pedalar = new Pedalar(); pedalar.setNome("Passeio"); pedalar.setDuracao(60); pedalar.setDificuldade("Médio"); pedalar.setTipoBicicleta("Bicicleta de montanha"); pedalar.setUsaCapacete(true);

    ArtesMarciais am = new ArtesMarciais();
    am.setNome("Treino");
    am.setDuracao(90);
    am.setDificuldade("Alto");
    am.setEstilo("Jiu-jitsu");
    am.setFaixa("Azul");

    Danca danca = new Danca();
    danca.setNome("Aula");
    danca.setDuracao(45);
    danca.setDificuldade("Médio");
    danca.setEstiloDanca("Ballet");
    danca.setAnosPratica(3);

    System.out.println("=== Pedalar ===");
    System.out.println("Nome: " + pedalar.getNome());
    System.out.println("Duração: " + pedalar.getDuracao() + " minutos");
    System.out.println("Dificuldade: " + pedalar.getDificuldade());
    System.out.println("Tipo bicicleta: " + pedalar.getTipoBicicleta());
    System.out.println("Usa capacete? " + (pedalar.isUsaCapacete() ? "Sim" : "Não"));

    System.out.println("\n=== Artes Marciais ===");
    System.out.println("Nome: " + am.getNome());
    System.out.println("Duração: " + am.getDuracao() + " minutos");
    System.out.println("Dificuldade: " + am.getDificuldade());
    System.out.println("Estilo: " + am.getEstilo());
    System.out.println("Faixa: " + am.getFaixa());

    System.out.println("\n=== Dança ===");
    System.out.println("Nome: " + danca.getNome());
    System.out.println("Duração: " + danca.getDuracao() + " minutos");
    System.out.println("Dificuldade: " + danca.getDificuldade());
    System.out.println("Estilo: " + danca.getEstiloDanca());
    System.out.println("Anos de prática: " + danca.getAnosPratica());
}
}

 
