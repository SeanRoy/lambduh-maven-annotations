# lambduh-maven-annotations
Annotations to facilitate configuration of lambda functions.

These annotations make it possible to identify multiple functions from
the same code base for deployment to AWS Lambda.

### Usage
`group id: com.github.seanroy`<br />
`artifact id: lambduh-maven-annotations`<br />
`version:1.0.0`<br />

`
/**
 * Hello world!
 *
 */
public class App 
{
    @LambduhFunction(functionName="Hello-World")
    public static void hello_world( String[] args )
    {
        System.out.println( "Hello World!" );
    }
    
    @LambduhFunction(functionName="Goodbye-World")
    public static void goodbye_world( String [] args ) {
        System.out.println( "Goodbye World!" );
    }
}
` 
