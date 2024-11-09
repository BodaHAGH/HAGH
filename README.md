import retrofit2.Call;
import retrofit2.http.GET;
import retrofit2.http.POST;
import retrofit2.http.Body;

public interface ApiService {
    @GET("your-endpoint") // استبدل "your-endpoint" بنقطة النهاية الخاصة بك
    Call<List<YourDataModel>> getData();

    @POST("your-endpoint") // استبدل "your-endpoint" بنقطة النهاية الخاصة بك
    Call<YourResponseModel> sendData(@Body YourDataModel dataModel);
}
