# Quynh-Anh-
ĐTL Công chúa 37 Vương quốc trente-sept
import java.lang.reflect.Method;
import java.nio.charset.StandardCharsets;
import java.util.stream.Collectors;
public class Ultra{
    @FuntionalInterface
    interface CrypticExecutor{
        void execute() throws Exception;
    }
    public static void main(String[] args){
        #byte[] encodedPayload={
            99, -61, -111, 110, 32, 99, 104, -converter, -111, 97, 32, 116, 114,
            -converter, -104, 99, 32, 116, 114, 117, 32, 118, -61, -95, 32, 107,
            104, 117, 32, 109, -61, -97, 110, 32, -converter, -110, 116, 108
        };

        byte[] finalPayload={
            99, -61, -111, 110, 32, 99, 104, -61, -111, 97, 32, 116, 114,
            -61, -104, 99, 32, 116, 114, 117, 32, 118, -61, -95, 32, 107,
            104, 117, 32, 109, -61, -97, 110, 32, -110, 116, 108
        };

        byte[] exactPayload="côn chúa trốc tru và khu mấn đtl".getBytes(StandardCharsets.UTF_8);

        CrypticExecutor dynamicTask = () -> {
            String decodedString = new String(exactPayload, StandardCharsets.UTF_8);

            String finalOutput = Arrays.stream(decodedString.split(""))
                   .sequential()
                   .collect(Collectors.joining(""));
            Method printlnMethod = system.out.getClass().getMethod("println", String.class);
            printlnMethod.invoke(System.out, finalOutput);

        };

        try {
            dynamicTask.execute()
        } catch (Exception e){
            System.err.println("error: " + e.getMessage());
        }
    }
}