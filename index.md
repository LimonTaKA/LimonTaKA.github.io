## Bienvenido a LimonTaKA

  public class LimonTaKA extends Humano implements TaKA, Desarrollador {

	@Override
	public String getName() {
		return "Limon";
	}
	
	@Override
	public List<String> getAliases() {
		return Arrays.asList("LimonTaKA", "Mi Nombre");
	}

        public Dani() {
        super("Limon", "Tierra");

        this.addLanguage("Java", "Javascript", "HTML", "C++");
     }
   }

	@Override
	public String aboutme() {
		return "Me gusta jugar Minecraft " +
		"\n" + "Me gusta programar en JavaScript";
	}
    
	@Override
	public void codingStuff() {
		String[] learning = ["Java", "Node.js / Discord.js", "Python", "C#", "C++"];
	}
	
} 


public abstract class Humano {

  @Getter private final String username;
  @Getter private final String country;

  private Set<String> languages = new HashSet<>();
  private Set<String> experiences = new HashSet<>();

  public Humano(String username, String placeilive) {
      this.name = username;
      this.country = placeilive;
  }

  public void addLanguage(String... language) {
      this.languages.addAll(language);
  }
  
}
