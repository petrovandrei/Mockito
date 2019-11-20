# Mockito

## Configuration du projet:

### Rajouter la dépendance maven

```
<dependency>
    <groupId>org.mockito</groupId>
    <artifactId>mockito-all</artifactId>
    <version>1.9.5</version>
</dependency>
```
### Deux manières possibles d'intégrer mockito aux tests junit: 

#### 1. Ajouter l'annotation @RunWith(MockitoJunitRunner.class) à la classe de test:

    @RunWith(MockitoJunitRunner.class)
    
    public class TestClass{
    
    }
    
#### 2. Faire appel à la méthode initMocks dans la méthode SetUp:

    @Before
    public void setUp(){
    MockitoAnnotations.initMocks(this);
    }
    