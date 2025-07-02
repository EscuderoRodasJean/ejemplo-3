# ejemplo-3

AUTOMOVIL

public class Automovil extends Movil{
  private String Modelo;
  private String Tipo;

    public Automovil() {
    }

    public Automovil(String Modelo, String Tipo, String Peso, String Marca) {
        super(Peso, Marca);
        this.Modelo = Modelo;
        this.Tipo = Tipo;
    }

    @Override
    public String Resumen() {
        return super.Resumen()
                + "\n>>En relacion al Automovil"
                + "\nEl modelo: "+Modelo
                + "\nEl tipo: "+Tipo
                ;
    }

    public String getModelo() {
        return Modelo;
    }

    public void setModelo(String Modelo) {
        this.Modelo = Modelo;
    }

    public String getTipo() {
        return Tipo;
    }

    public void setTipo(String Tipo) {
        this.Tipo = Tipo;
    }

MOVIL

    public abstract class Movil {
    private String Peso;
    private String Marca;

    public Movil() {
    }

    public Movil(String Peso, String Marca) {
        this.Peso = Peso;
        this.Marca = Marca;
    }
    
    public String Resumen(){
    return ">> En relacion al movil:"
            + "\nTiene un peso de: "+ Peso
            + "\n Tiene una marca como: "+Marca;
    
    
    }

    public String getPeso() {
        return Peso;
    }

    public void setPeso(String Peso) {
        this.Peso = Peso;
    }


    public String getMarca() {
        return Marca;
    }

    public void setMarca(String Marca) {
        this.Marca = Marca;
    } 
   }
