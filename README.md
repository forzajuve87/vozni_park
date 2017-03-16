package vozni_park_vezba;

public class PrivatniVP extends VozniPark {

	private Vozilo vozilo;
	
	// kostruktor
	public PrivatniVP(String adresa, Vozilo vozilo) {
		super(adresa);
		this.vozilo = vozilo;
	}
	
	public double porez_na_cene_registracije(int godina) {
		return vozilo.porez_na_cene_registracije(godina);
	}
	
	public String toString() {
		return super.toString() + this.vozilo.toString();
	}
	
}
