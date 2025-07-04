
-<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>R.McClure & Sons. |</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        .hero-image {
            background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://images.unsplash.com/photo-1607860108855-64acf2078ed9?ixlib=rb-4.0.3');
            background-size: cover;
            background-position: center;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }
        
        .before-after {
            position: relative;
            overflow: hidden;
            height: 400px;
        }
        
        .before-after img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            display: block;
        }
        
        .before-after .after {
            position: absolute;
            top: 0;
            right: 0;
            width: 50%;
            height: 100%;
            overflow: hidden;
        }
        
        .before-after .slider {
            position: absolute;
            top: 0;
            left: 50%;
            width: 4px;
            height: 100%;
            background: white;
            z-index: 10;
            cursor: ew-resize;
        }
        
        .before-after .slider:before {
            content: "";
            position: absolute;
            left: -15px;
            top: 50%;
            width: 30px;
            height: 30px;
            background: white;
            border-radius: 50%;
            transform: translateY(-50%);
            box-shadow: 0 0 10px rgba(0,0,0,0.3);
        }
        
        @keyframes shine {
            0% { background-position: -200% 0; }
            100% { background-position: 200% 0; }
        }
        
        .shine-text {
            background: linear-gradient(90deg, #000, #fff, #000);
            background-size: 200% auto;
            color: #000;
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: shine 3s linear infinite;
        }
        
        .floating-button {
            position: fixed;
            bottom: 30px;
            right: 30px;
            z-index: 99;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: linear-gradient(45deg, #f59e0b, #ef4444);
            color: white;
            font-size: 24px;
            display: flex;
            align-items: center;
            justify-content: center;
            box-shadow: 0 4px 15px rgba(239, 68, 68, 0.4);
            transition: all 0.3s ease;
        }
        
        .floating-button:hover {
            transform: scale(1.1);
            box-shadow: 0 6px 20px rgba(239, 68, 68, 0.6);
        }
    </style>
</head>
<body class="font-sans bg-gray-50">
    <!-- Floating WhatsApp Button -->
    <a href="https://wa.me/+447801959777" class="floating-button">
        <i class="fab fa-whatsapp"></i>
    </a>

    <!-- Navigation --><iframe 
  width="30%" 
  height="70" 
  class="fixed bottom-4 left-4 z-50 border rounded shadow-md" 
  scrolling="no" 
  frameborder="no" 
  allow="autoplay" 
  src="https://w.soundcloud.com/player/?url=https%3A//soundcloud.com/lewiscapaldi/wish-you-the-best&color=%23000000&auto_play=true&hide_related=false&show_comments=true&show_user=true&show_reposts=false&visual=false">
</iframe>
    
    <nav class="bg-black text-white sticky top-0 z-50 shadow-lg">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center">
                <!DOCTYPE html><html><head><meta charset="utf-8"><title>close-up-nx4_with_bgc_cropped.webp</title></head><body><img src="data:image/webp;base64,UklGRlYqAABXRUJQVlA4TEkqAAAvX0AVAE0wbNs2DBSvDlKj/x/c7oeI/k8A2AC2P2zu7i4ANzl0rudMGfxYU4tfTSWhgUjU4bkUCkkzW51k68xIBRgQUIEFg0aSFFUmd//vXyszioAkSbaqKnGHHuFy978s3L67DBy2bSNJnN3tv957rf5PAITQpuAnhAKOA2a0vYEZeJzzeuQlBAAw7WlnHz/xRwTXwBgBCAEPU+p//gza1IWEkhSl+i8I3UAUKSlZlmHyR6JY7KnOVJkq4yATJfg1r5rxQkDwf/m/igraCsj7sh3g++HZ66cAiK66vI9n9Xi/fZ/d2WEoaNtG8sKf9e6hEBETYM7UPHpQZXfWI8ml6DxZkxrfRdEaxLdt22ok27ZVa2tdXWBmThExaTEz89P6XGZe6weYmTnmjJgxw8PdzNxkknprdcFP+JYkyZIkybaIWPPy1X39r9vMfNG8pwlZbiRJkCRJ1aIWu//jn9FDp2soSNuAEdHuSPAtSZIlSZJtEbOYefa9+w/6//+l+y/ur3WvMlOhh/gJh23bBhKV+/03/hpi2LaBHNDX/SfuR6G2bRsGXu308gPm/f8PSbI9qB/jF0yWOottG+M551zb1s7Y3bO8XN7VXdm2zfG03T3tLnc6MzLD8cP3wrckSZYkSbZFxOrRF5h/nlm3T75WZbiQb0mSLEmSbIuIRd0jsuqx/v8n+5qRbiocZfjF//9fQiLKxAIksNvtxJQ65hCGLgIUK2Ssw5JcUwFAiF+3wJh1dk1aewmKxcC8vqUMXZYgiGWzQOhd4H/6HL5wdhQgzTNYJlJbBhAHSaC3/9Xe5xk23s++9R8PuDnwPYolPcCWE9/O4miiKw1onSHC22vRjmKVWW3ZQDSGtlcsMLKJCsQvWwFGqHNtlxmvbSrZ0kLH7LKw1PVEYhCmQCB6hcJm6KGn5iJTJUSMnDnBAAINtf3zkEcCZKsIXuyTfY9zb9df9vsr6OsJOvDZcR6ATbLGTRwIO79GrWIJ7b0c4u2cjbGchmOxZpuNZgIIaJZ0yHBZBywWJFuyFtJdDwFGYMiE5uRMzruW7q/xUnIg4i0ZAgGo1OgznT3hlm2jHVjl99F/aozxQEffwb/vlz9oODhnWqDzjOwYT8ZJdZ28PGtpANuzACUAlgXayqlND4cBsIHFQE7TKVmgjEgJy1vh83QgQdh8MUMTDBecfWWmhqa0vYhQQEwR5G7MJ9pGq9xBW+ut9XPoO+qUX9Tvmm9PYzyMQqUM54p82uxZdlX3pggrCV6qRNgKxZCILAGD5TBWBQxAMCXNqDLdiLh0WFRTb7mY20MvNDFFlRgACV20MEjLwE1yggKgDQUinonoS82QfJZ/KA/9XQLs7wfLBaN6GKGAQiCc9rnV6kHnSorpuWhKJHSY3tqypu1sMrRMAs4prFctZoHFm8lqVRgAns5iqRBg8642JBIZSAqQYIhm7aoEBGJIBAueRDBlas1rPsVFAbiVu4LN1unb9O237e+az3FqGT1UcPAQ19iMqZc4gQISaWe3LX5IDjuWyQCBEDKbl6RMEhuLMFtSV2OAKA3pINQQrEEzChIjJaVJUOKGrgSBAaF4wYIAWyKg/8L/umiaQsWj2cbfwnfr//v3uWfS91Eu7Hhcg+4i5Y5WLivd1LpaF7VhjNnZCsCsNqNYBtlCCGE5IUlpg5XFSCYFsKKxEGC4WoKgQSyDhGCbhQaFSw2qakJBgBSzCJBBG4bv8TO0iJiHed13f2beVob7mWq3p7Rv+91n+XlWO5sw0FRW57ol1ZVk2erDbm0r12XBJWRWAIOwkEVYJ0ssyiSyOEu2O9EmIxrQRaulnfNbqw6rjSWZD09vREeBag8iFAxLfLgPsnQb/23vz4tcUwPtQU7e2Te57D7f5kOysqh1Ypbt1m2EMJAF1oKhmcQSzAp5WHtlWAYA5Ogo1AIj8Lkb870UY/zKu82yCi+vioZS1zaK0TttFgqOAgdF1Ie/rIW4uGtj8ufr0W+AO21/QUAAdjv1G6cuPmq3srQuQGZ5uke/6mP3ntIgMixrthamHEVlU2KxAGKY7rhlqghsfbbb0xVjw/aljFSPxuLGGyv23nutdI4bHBUB0Fa9mFgJ1Vi47tv7F4z+S0ycjcuIguXlaKtcRLs72dosSi1jIYw3Q8eyA23DjBWlnK2CMKrDGBRt3g3dHgrLxU0QAIVLIF3KXCocz5rArG7wUYAQKBBA/++6GXQf7Zed78cO+on39vf7B3mvs5bjHAJRuqNHByZ9jbxzCnRpsbxOhanPVpaAsOUg1RhallgBLPpihac6t8Eg4/2Ot1Z9a6rSULMt05dbbE1WW6qLSgFBUykHmtfW59fWz1tr7btf43FP/PtCJsdFjDi7nQELmGU5HJ0OL+pmH3Z0LJld3XgNE4YgQdhO35HtUkeWZdIFGAQI2m/ud1bK+PUWLgkMc5qoxFmTGsDpragkfiCgFLiD1N/Dn81dR9AmfuXPms+u/pza30Od1MIYBzZs6aICFssD8Oa3ervUTQBUyhAADqGKCQAcHQ2DxSxDwABDsfDo4rJv/nssNvgQCEBWKlKtIIzmQvVSKcIRDP5KfoH+ZnVUx/nZfV7WX2PWv4O+m30ZHnu02q1vZO873eHo7Y5bt1k2EsCwared3SZEAEHk1KwxEMBWj4arWPDmWjGIh6Acwu96Vy9AyEATAaQAtFESTnaB2yGakPa37lf1D/nT2tdrd+B1fIuvlmle9vW1taLzWSv3NpItO7LsrE7fSlMiAlkJZDUX2bZbBCCEAFK+vs/FI2oINBn7CqVDFjyAkAnAQCgACoEjtRCaCDSoNJSiyGI+pP/y6a33lK1nRwZwdbysqZkjJzzoV9deeVt/+yu7MoYO2KBYeLCdI/C1XRkKwlczrF1aCQCihgChXCy12oBqbaxMkoYdlRAgyRAAUAAUDgc5DAQGQVjFOskn7MPXx6u2Hpix+OJrbbSP6aZMKrQ23nNnvuok0mWwzHZsHBa4XBYG1teHESsDX8A6sW3HF8VQAGsIAcrFMpSrp3pjsiEq7fzJZiYwBgKFYsBhAGnIyYYNErbrI/pMyNY9DFrWGSom3n01ktEm31lzR9unsjpbsWcNhlUPP/1lD0gSWTwKizyIcW0pydpOJICK1X/nueOqRahg5LaqxItL6M1teqtuyZft06U6ICYTAoTKJ4UCKTLMmD6Lx7S/JbIIKkamZnVrMjZSQ1H24LaHw0V+ty1u8XwO/rRfnr2oppOolparMBQYABerBi6P8rGD7CHAQkiaKitV1NgQ2tpmeWozZHVtX5fc4RTpJKnuASeQ5tBNbk/0p/SETQcHxxaZBH45/Dq56hPJYNSWcJQcc75c5jZNz3J8/POwbX1mrG9RnAciKFc/AjksgK2MCV+t7uo6a1tWsIAZOrUEmy2luk2vLZm9btQQ3HIVkgmLhNIEijuLW8e5XN++BP/A95+zM0ploiBzQ2bmcbpzaCxm5yXQZZl0vtlTec/fpHvu4+k+d2+PfG/9JXhEmUqBX1UzXiCIAbOH1QmsINTP59f5C3deQoZlklCSc8dcZm199qiQ1jsmNbZ0BhMysimM3xfCMIR+evyb/AcdqaOR2h6jpmpbqqdNbJ8GB6P8sCD19TFccqo/P3/t439nlb22iJ1DZBvcn9rL5t4tXWJyd1NLyyWZjSQSxtBBwo/6V8rf83tbJQKpVtVrZA6su5K0VKqQco1srgkAhDLthmL7rvf/3r9y71PQGVXkYwdJjFxTxTyw18Lau1w1K6MKkm6w3Lwt71HCe7X7qSWbw5rsE/z8sVwt1+US8KseRDAFxbOQ+RkAJToEAAG0BFemUuDS9D/PDb5h9SABCBgUCwDAKPCSIbvCABAIKiAVFCAEQf7fIVA2WYe2s/ZoPG3qtHJTgq4QBooqjtYlYNbTvTNhPGySmRxQGBp6i3zHJMEroOGIN90d2iP/1JqWPcxukHNKvMYhLRYECBP3KNQMJQEAdMLjf5n7f5CPZ8grzTBIYUAIFv+fzBcAdGAhYQg0SQXAwCdF0haS0NGHMY3cSKc0oyYGePhtjlP1KqqocMSTLeGSSWYBA11qaZ/etvAKLt0j2aLrUzIWYB87lBG2UCx4CzgzYvBHQBHI1AYJ7hIoJAJU8f8AcwAkTIEE4PAub2M3AggMipBEIABRlIAABsAkoAsLMS1HMvu2M8JtwWpjsTpDCLsa69ETW0+zm+hQrnKT1P7aXytz9vm6/NDu/g/P1/VtaHlDsefT3u1GzAaP5pvwfdGdaDvzMgsGQD9YydWbTXVpsFqFaV8GdmCI8kyRCI0IFFcTRFMAkrLEx9sbqSYkmRIQBAqDQPUiUJQbXeT4HLLdtTviwe96kx2KlKKuoEwou8UioHgQamOoVkZ1ILHWZZ9gd2eurOtxp4JioUyjwBoRM7CHXXa6Iamxnv3K3uQvHv3BVgKtt6WO6zQVECuxqmh3R40Bb7M7HAc0YCIJgCIUpIELqbRLHPGWqpgKTAQJIMV1nOkM13m6TmO201oGUAr16iLKMEsg02oJNZDQUIAFKPVMidxiLIgQD1KyA+v2WVxgq2/vPALxkGFwEB++ImzIPC67kq2ynVm+v0/1/Znc/jvlaa4oAeigVlOsQ1D0jA3sfFkOI3Q5jJLjzVmh7qCm4xe1I6mlWSqunCussOnKd3qssXVXMHjOSx/HPgZ1RHFYlnSkGF+pOlRVddVKkrcW0bDzOs0zm8v7f5ZY7cEBC5uNWGmOua905IqFfXReyoVQHiZ7lpryxSUvwYMF7t/7M3xn5PfTX4Eu/6zLDpthM6EINKX0adQec93dnxf27PfEn7SPFRPNiAbGKMGZIAgACijTsAQpfILxbg8rnrgnL93WFzkdsSn2gj4EBF4rCkF+2JShHBHtSyiU7G32v25v9d0C2m7CUiPJU+eYXVi7oniwK9/mb/tLyQjEAVdT8uytTVgD8/3zoo/QEne/MPnT/5Mv/4/f5/65i4w3pjj6JsFHXegFT7S2mZ3GI3f2m+10b2DjYbjQXr+NTq9PCopwoGQkNtrU0nD+PvoIysVEr6bXs10hAtd3yFJ7JYIDGwSKJmMEoZVajwXxoLKekmOxKZ+8vWX9y7Qzr9c/+bcNkmRoRP8d9N/IahoGsZI3TWXUSCMrhuD02JuF0m5jasb1Yf/4/Zz7mBNTD2bbVjtBbxxNrzDHM/v39ghf3LR12qqk6FsNeG22Oyq46ZExeWY3GjAVxq/OUa12BjADyzQIl7XmtjyHsdx/O19PXu+bzJiIZcRm1mdmaM3K2rZDcBchmOaTw7tfgq9bzNaMuN097V0AhFRSVAlYrQswkmEtaUENaeXDOOR7j8dAdUz3+qz3Pl8e4b/KvQb6nKx/ePTxELfnK3j1fJAb7uDtAME4X5R7ZBMHOAF8pLMuyGbu6vs0N5fKd0HjysEGfjDqVrNQYFaCtIkOacr2/8HHL5cLv90HI4HpHkQYWKG0Z7ru5FusbmhEAOjk3EOdAyMjkS2du1epRAgAAvqmrgLWu106w7gaacHeoF/q+RLGN5SNNLjn7f4T/4JRbISncVYveCZUKzmEYXUTG7kbCGJeanNu3WbuZWqza205ugdrrOE/L/5fm/8Xo7FXjx0rf4SjiJSEj8FaisydmX/uVIsv9vu0F/s3+77tf43X2CrAM7OMUnDQCksn0Q5rYIrCNQvXxwZRhBhbWcsBGkqAgEMZbbPPV1vqxMEKzBxKv3KvLyej9pYXRjvWtrXPXf4lBRM0wLXBdejNRosFt3qbbVwjAAYDsCym10SkO2f47Gc37FNNgT7z/xT9p5NJ7MK/rvjrnXy1flNmvI0/CyC+qpYMUA3kxGkHIgka1tE61fDMJ56ClsgvFxwu4d3+UFXmURQZvlorwSI7+njN20wTUMHmeGSk1ZirdTSDaOaL3kudj/Rv3rP7uXjmWIZvjh0NpBHT4chQqwbBqilrBDj5Ci4V6EqjrDLsWg5d/cczYjwqQCKbQmyEGCq/pZMXRE0UaoEABCQdMTWVzBVYLxzrgOTV22id/5sYd3AZZ9TU1IYyBYn8sqL3LA93WAAkWQ0QpdWHheITQRcJd3qkgckyDWEKdzKt98H/wDgyKJScm/xNhVMHnEoxx0gTHGncVYNeZxxxLA8UAejq2fqPXXYIgMCOS2JkC4GQIlcjQFEgZCJZmmtsk9nwVGmDtrfmDxgjd7hVloptc7OMa19EJ1yyrslNGUMOWnFiOFoWZN0m0UYT1rJS9qQNRp3su0bK2KX2cOeryJwgkPDXr9zPO3tQ8h59y+jlXnf7KxgASE2rTVArQOStnKqsOipU4wsKp6bK6Fh9BYhsPiG/Cy+AZ5FKkaKVVpZMhSnqsZ5vqYGf9/b1SF2Lv31JUKEtgcks9jBaUIYLUkhko6pIFggQIAxwKXxTt2e4L/K6x7smG141dMeIJVQunnGJdBYMZUdKSvPAUuWubss5gF2TOHmYBaf1u0wkoiBuggWaEHDVd/JF+/BcD1s+StBPqNcBOlK00qV06mi2ASw+5jVw8RNviywBEGNSD7GAY8xchODwXACLjk3axnS8i6iJo5zcu84yiQBVghY2dP7WkuHSAUVMVtgzVeIu2cU2pbDAVB0l/sVn5iHFSbpMDc266L57z4butkYLC0bvYJkeoz+b2Im0c0aQlIR1zwbrLF/U93GkZpRiAbBYe9IHX21TQTFf7x7XdxcjqDB6VTguUbV3kMXDUQ/nN9PnDqcxrvKJjUdG4/mkbUWrbP8oa1aBMHQigo5OQCMLZeohpF2k4dUvc45jHfAZQZ1tBhEtyAwjBvW+5j05Npix87X79D6JcPpdACiYVl4b1WDrBgQKiRnTkODIR8Tz8XZ12FwJixRYUCxE6ti7QUT3+G9+f0OTHjwT4DkfsyrCx0r7APvahUPEQUvN2mE2Nrdf7u9TPSTEn9ppBdeMjKrKFIFyxSeB47MoHWsRdFgjJM9PN/dMy55wWC9nNhdYV71fvqb6H2Np/ePlU9/bJTwRqgO7SY2PFkXKNEBAYlJMEnAYQhx6GZehD57PrPxWiqkYEKRmSE3qY9xdu6ODGo3T58XjcF3sOoKuSOEFT/riXvS/9T/o5ceuTRFfc5qzjiIYAgqOLM8DGiMcVqkNnL0+I3xYWiHj0xpmxNA9/pGnOppNSZ3dz/sct72p4on9vjgz5uhOU1Ym1igN8phzBUivvlwAqUwJxcPMR4VK8WNbP7Yjj/wsWfnTItRvGwOIBGGS1z8P3/eyMQ9HLMc+Fr/uj8M089M4rw/0Ud/CM2yFhVLrIgzBKibb6Lau8mZEF9TIAMZnTrU5pz1NzhwMs8czd9Qy3A2FFVU0pevp3a/xXlj/HR64l3Rzbo0Px77dRw0FiAk0szkRWULUaXUYmyZCzTPpoF89zPBOPz56iSr8CBZ+av1jrf830796wZmu0rwEQkr346OYlNJSJS0+deOOXppfqRmiIaECHSUYwJQDXuZyX8NxO8N1QMKqbj2zR+vzjVpj3/e8itmGYwnDUor3ar9L1zWfC/R5+ZPOWembe6Nhr8fcdRZ/q18POL6M9Nj59RvQ7O8GnEVa2SZrelAKTH425/yg/zlmsB+ZfxUEwoD+gk76p0YD12wS3EabNGpivT95REkUAwIKBhjuvEEZgASFmZgCEFQVHc5UTNciioNAJee0IgnJi0c0rctMDEuHxOgwwX0RnPO+xc7QNXdztNxLLGMe/VrLc7o0P37+JW/BE8LXOj/6eXWG3D5bnK55TPdb0Fxd+07z/PGl/R6l7eDZL/A79deovyVQUlkBTCiSIpCBEL6CFszeZnvkoQhREhSIWFCUgcpmIYYguho0YcH5TscdWJPK2FFBG6amV4NynFQsYUPcYqIUTcCLrbP0kj21+y/4t/pl9k+fkR7VxhznkSDjX0tffDdhfmDnh+anyy4P+sX91/nDZ2OJDbuGdy/yfj7yjgdG7ms/Uca59sy3aiqQrhZNdTCaIEsRJaoAEIJTt7qdKQOjryoKASQIHPp5D5/XO4AaY4zTOoqTTRjZZwXRRUOOO8Rks55c3Ghj55I04hOviDJ/9/z21G5Wzs5kfdetnj/1b+/KEpz4+M7bDfwHTIzJpPnBl2+eH5k7+3ij4Khv/lv+2Pc19QJf5s3bDIlacTWgFRAKgLEQRmDiQOAA8w4uZqECEjAj1Wj2NsIY5ho30h/TW4GVdhFW49Dr/s/uuWvX0c7TcsXzKbfbGokoHajgpaILSGfNdWJy3fHJjN9p7s1lFt7a5819avQXyW9dT+JP/5v57R/9PyoayheqkRfrEHhlU9MfMa8/Xnb+hNZ/bmUN3k/79zthpt/zt4jRqTSRRmlFQR3VFoIVB7U+w7m6isVlL76f9/7+9W5UTCVAiCCpxOCCPF+x5n40fvL7KjSgNdJavTWEl+Yec99sQp/FgIEMT4zGdJZp7DiszYZm5xrXxYfdSzK18TqfL9vTfjfzHt2ek75djv+I31rb8X64KvF+LbiKEnQIe5yFtv2zHd9beCrvd/3nX1u//wSLfLn7+ud3w09Ve8OJqqAMuQgHsyXNNXAqULCYkjuO65Ozu791GzAFKQUQJAypQVPjHuXsHtkeunc7qzvPR7mpg5GFZikIcQi3ttK1Aj5QRuIYdk0EbrGHAfc9yzff9j5Lu7+Tf7++HfH6Fiv1l/7qBeSvp2BQH+KO4Q4nhnqzTiDG40+WeFRJEcrIBojmapD/gD9LE2QxpKIuPsDoPweYzi6t+m5UbdCW3khtj8r43Xz+VkwgpAFBQCgjIMTjk7x/Q5Upn0VLhLZmhVCYU4z2UovFx9ICl8nxaunQAl3ieIhm3R6dvvtFPLf7b9DRL8JlvcZ5g/s784a9Tr/6de7tzW2oC1avxBQUQE0y/8Dke2zN7lRY/CgcZpPWGZPyX7tAZEGpuZNJCpKTF1w9YMgQwrSMGli/PCInffsHKQBAkgMQICRqg84SagnVqsJQAwQscRiu0oKtaQ1szI/26BkATwQHOt44zq54/8Of+3yaq4QYcv0Ej9nPnLnagq8rub1ir7qGhUOCtjEMxCS6mFjH5vR3DfL0PouB/57IBqqOpUoJgZBUaZmx0Ds8CPWBWFEplFG+j8n8AFHvhBdy/P+njACQY0izjIlHaGo9cdRCC7ElT75WcZ4sn3svH7/+3R7ABlgVMbN6mj3iJzU3te1HyAygI9Nb7EnYT39DXsaXrdx9rx1e6hyDNFGU7FZFmA+DBKqTvlQoPPAZ/D/Yd6cviYEAjsBkFCHROvWv7ndL35UqWWuXH/ahV+a4MrqCUDojemeAAhAUgABgICU0+hr4jpGHgKmvceUun5XrHC5dWmfV4GcuEG33hhuSppy2K2x3ufLmDkQ9xPrGXv2fpyM/KR+uBX6JW3L/Oy8jx/r3VfF4ixS17rIZZiRTCeYgn7KnG/ZfsN+O30x+xrw0TSEQmwoBHDIzKG1OtDCZhxnXKy8c0FoW7S0uooBFHBa3KAFikkgAQkFIk4W7w8xDAMKTuVw655nqlU4JWhAAGKDCRFgNT81Hn3mMhctbKlICEW4Xh+jA18Qxuv367+zkrHOwFDQGDUzTYTKK7Mo/qJfihg3nb5w/JB/ifzL3z+uIz3Pa2mxWrw+gkNhN66gT/8uK1uReA/oXn3jFTnQtWvZsdizj5EwAFGmiMNDFJJH6bbNlguvCMSs+Wq5+ow0GIoQaFeBVrL3NP7/fP37v3/5fu1uW4FLp4YnL/LcmL3ZX5Teef+l/Ox2P1V0dZzSPGv5AfbT8FRhwWiv4b/j35jP5GfHBv7gfi1uLXTCKvWceFzQT9Zx/p6Dby+D1RUfbx74xOna3LdeRg/MSFn8YM9lYT07XIr3s2YUu+LDVj2/be50yahBRpPSVWaJYidrAbWI6eJs8xP/59/bZ0k3fb/tlrUvtlBzOFj3+7vubX9hc1/uUb5UtxnbnPB+zaq88Pjmt37WFBMrUyI9iuMqAQ2G80zjiKmYHA6WBTXgZSA0qN5otuKE8RnT3FWLd9s+TufX7p9XZ28sPiltxD3LWd/IvuP+o+KKQI+Zia1uy0kktmQKEqmwvj8293JG8pWtNXO1SZ49lTUSZ83L9+bNv/thkttlkb4WcpRtOoYWiYv+j2NfMA0pfySKeLqAuM6x43kLgdKiJ+aUM8bCQUtFUfQGZLAWPnz1PbqgN33PGDKoa49hsJ98HW03ypvvTvX9Wx4fIXMA5+dTLQXjL1raW9SjgwHnxzRNny6xyH6Cq1ij1AWOhmoSjEK6Pv37+MhnQeUBAShNPsIuu2umAS9tGOsqFvyJxXW8gkEGEnWRt8Jv6pQrpHksrYpEuDCvY8Ltc1SAgkjEIqZ1foH9Z8xx7yZolTfQw3/bofZbe7dfyjQxt1jRWMgiowb3k7Vf37cb1xZ32koXtlN3UZspsoQYiFukAPHWEdVM+s3WhMKZma1773OAsykEqzEggQIC/pYVb/NmsCViw7GF+w0hlDypASOtwVZgFCQXgG3ujJwHNwsFFFMiYJxgp0WlDSoPT1kEPDe/cvbf2GkhVQrlEQEBknYt+kYqvZthgO502XZHCFSG2BHWiJ0e3PmZQZiVjNTqHgnFxPdYk7iJ1AVA+yCRPCCz8VYK1tXbpxQJkBKAw6rNqlQyXwx/LVlFLFnFlVVOTekzXiHQV+l7wW/cVv+RtZwSEI9khXpnj1aGTS1EiEgFSFQinQrynwVffD7KNJfEMuEqxhYIoplbm6NTFh52ntLYch1DXV0OsZtSNqjjBGo2YSAibmBLkqzGWigM/CCGVPAn6rZEy7GWhEuv+iiCNWhBFFc3f5KwWGwv0PKMVFiKkrj3vtKFsvpoH3LIpSZiqSAQKFsBLQyscSvVjlzVXTzjZotoCQYLCKIeLJypET/v9OlDII0KtYeTbkCezE3R6ceHkEIpGWoiXqmZMISseecfRYAtrebHBOXOqFyyX2rzmrdlA7wRNmFeh4gqPuGpGCQuklQYNspMRE5IAABAAQKU0FXrc4yCpaPnnKXPUsbgUCoRAGKHP1IakcF2O0nBOTFoDzcY1sdjjA3ywDQxoycB6lYX20WZ18q3+22DFpZXnMKN3ne1RSwJta6HC0QG+4HuhFsIMWfhaBMGgjSVCARUnX6lWITQAkEDhFi6owk0YGzaiic1VnASFd9Vw4TNouLlt77TNCFfd5Aq8IGVnHQYghM1N7x1y5T4QEJKQzqBgjnrtKx7u9i69a/bw8LhgvdpEF1QeRZN8iyesvLZ+f311niADskGAh0SO2CDA0drgRhykjQYQkZBGc+VdK+/t2B4Kx4sKcFkmZvjrdXUuX92+6XN1prs0GuCz+iYHPc1Vx1H0girKBoTbdLtYA5sKGhSVersbMMJ/MOjyscKqE9/0WAVcQ1qxXHbuBidJuQh26W++4BDSTVWkDEFj0bMkgVr0hWiWCxdAOwmAmIDcxd1VA75QmsQ1ZBMzmutVXuuBmd7HuCfd8ORSn/QoDiOt+MLSCQJ2cYirzEbQVQY50+7oFlnnCG6Z+0oGrvaRKZs4rqNkeatqW2PRIKFLLn7cGwQ4A7hMce4KupSdi6genQvXHA2WAED4lGx9pAcYUWhA5ebAaXN23oL1seILfoRlDHCqIyy6h9dJ78D2vg3nbGiYyLqDDl8qkQuU3wdNngNXR3aCVc47Yw06MZ2kZAlw4c9stGShBr1VLUxy5vx8fkpHhqLgrBUApPCMJBuY92sOwFMoSYCoVmiuPlfVsjdXD6P6cwCH9UiAEigtqo1jv+dskC6rs3lyL9DcBRe1QNfgoDe+yzwvlVLLpsgA4GXzMPLvj5yBsxjhK9VHMVaMh+6xt2nTOdb9JlsxrfcIFYtGd2MESIuY5oESpOuxakAIAwBAkaM0b6m+3UJv/tr9/vqf6ccPQSs7j8BFXePRyzJzXnkf0b+7CdDFt7kLUISbJFA39fnV7rNy5EvCoCm3pFKcTKoOT0D5W9tWtY0VPYYR24YD6Dgs/BDo4LSjZjIM25JcV2tbBBauMJ0gieuUhkFMYDoRkC5gCXSDVFeEMXjdKiam1j3wmLbFmQTaBgxvgLvjlt204ya5q8E5JMoHF6xtr/TrgfJhOJ93EIuuGAhzBQsN3O6f1NjiJnKs0DuHhKaEMi3K9Bzv9nYe3T174gJCECQ5OZTCtAznzMxcdnJ/JOVEZQDkALAFlzh8vYayBQ/H+Ov0ln81IckEaLGQEmTMxooC9ISNxEJbOj/5KKIgxgAGRezbPS75DKiUBIKVAzFpkJ6oYsTV/jZ/wekgnikw9a4C8lXU8o1jx+yy3XNZ5ip9GzaABZAiFCP13kCdVHLo3E2/KYkCTQqEQdh0XR6vcXy/3HAZ2Mv+D/1dHTp2f9n0l8dTugoVQ/k0i54SpcHD0woWWAQEVDwB7+gLYfi0VoLiNHR06LCAP8cJqAGfUZYHAEGzoFvnC52GKzZcrJ+bd/KrZWv1TD/eFn6jr7O8tGmjQRJ9DX0cBQDQ2j/75kwixxAoiYIt8G3q3TF/A4FZsfof8/9qfxOH4NCLG+NCQkRQtbJApo1ZfyPGlEwdrdrgndrtvO7dPOCl73KfJB0JRuuKaGHLqIivnK6YF30qalC05XS+Cd4toI4RgHLlbDI73yEDYygmR2iDlC0ZYLD+fTyFwch2bUiQUD6igCHZrEGF6ayRG+8Y8CjJPt+u//oBkxv4oyfYcL8Gl2ysHe1AFJFGl7NN5K02DOrLm+98raeGsTxZeoWv8Pk0tEOiKTHpqRcG0sACRWHaCCSQzNba+E2Z9tUdU0ThqtI9qk4o9zmYt9XsR0SEAzBg7mWajOyAvpfvUbDJEUgtt+piaj3adLOTAqID3Ojk3iPk4o6xYOrRLOQHykSJwel79ZwI5Ibh3vm13TM9ls907hI5y0OORbCORnIq9Kq6Ie2rlwI8UCVPQtgtAlfoy6H3MyTdP9/WAFdnvGAj2ILBb0B2/Xjj7yzo2/ueDHyv4Y1Dt+tmfmwxrdgfQM6QfY0TG3oTFPG0mxkFYELXcHBPYWAXIRV6kSfvA53NgXKSTwwqLA0eB/Sd9tDHBO7Cs8gpa00YUVRUYCCxQoFbqmXQUM0OFwLOWuyQ31Zb/FNwNOK75QVLjgSFpSMH3Ku8m+myrdHdfqbcd994/tN40W/tvp4LFHw1km0AM4DbtmUMY4+ds7SgB4BSIGIJ4nd2SzdwoWZ9t5rbPgecTkSwC5kjoUfwG8lX0PH18vJgU1hOEVZ/wp9CisCwCxSiSP/8im5fFdx5VOEk0fx8TDO+OKOkwnGqAXYtBJYcGaVifxfz4u8N9JjypBPu8TnfjO/Tf6hf4P3QGOfB+yz3bfA5zbnINQIPVq0b5c3V0ss7AsFnL5vPxMCRYARaaq3eDeiuNoMouXOC+Xb6DpZv/l0eaOEK0QpL9GcRsGHAMCngsg2QX/Xy6p7heijcpgIRZuuIv8bf4JSKqztMLYwUETZwyzTAWNUBs64s1GZGzC5vO8xnHUDHBAzLFl0Ldq3vPe2YvUyRUSkH+EQIgBTUtPwRQkgA7sxkQ7hNJT0v9VZ5v8n7oE//9tN31kXOD26brbESrlgOLDWqIh49a4mTvD76Kpwk064yDxvGckiLdm8LeqqnND5x1LM5KDzIXpepT0BePmeEpRNKd9tN3v3pJ2yudlsotuHhHNYK7BzP7pP3tC7RhIeTgwQJB2AhpAMNGAyRLmAAe4vyTdNaruKrSldLEH2T8WRCITfMBynueI6pF5qlJJ/mK12L3W0/ixZT5d5SQ3ar2n7JdA17Y1WYTihiatk6ymf+EXVx0vGemJqBXDBz1U23c9KiaVVqwlAEFAoYgrY8j0/xSEdbYtNEDg+CwcbtLJ10Iqgz3npOepgqIeBYMJAKO3M2zKSavFaC09mYleUstwp1TiVwVjR/sJNBC39EaQ/+SFlPoqneDplYGZGVG2btK3j9Wj50W5a2yz0PKA1IgLTTWL2crYs2j+JqqFkALegZWBRxAGxwgaOe9Tkuucgyjv3d3N3SxA7bgOaSOTKWTDQhgJAJafDCs5B7mOSbNcHWZ8GiQteSC8+cD4CmDbPS1+0tLuzqkrvthZcjcIgwRNTowRzMWPjBydOZcB4dd/ZBCQ5yUC8AiDv1cpxZYb2Q1BCjCvvCQwSSoqSgzOtYzkf4sr2zK/Bz+zx+fdCr5fAdh0H8xIAFARaDCAZPc+M2rt6QW1WPknrPsKOrDv0NUiDnfvSoQ8xg5uVwK9jWJB3Cg1ypcWgYNiEWLQ1xVBlxzqugmgMQgHIWBtjgcIsCc2oyJ4zQijWhYdxtEhK52AatNf4WTRQlF16DT/os5+emrhQue2DBQKZBQEsMkoF66t1zlqr9QfbWfZfabUQZeVKn6BwO0ks/v7W+pr9/ff+Wy9wGu0eFtsUk1Ahr4IFCi7AOnrF+2o/lOXOAKUMBAA==" alt="close-up-nx4_with_bgc_cropped.webp"/></body></html></i> <span style='font-size:45px;'>&#128179;</span> 
                    <!DOCTYPE html><html><meta charset="utf-8"><title>audi-logo-1995-download_optimized.png</title></i></head><body><img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAB4AAAAUCAMAAACtdX32AAABSlBMVEVHcEzjHTgSGxuVl5haQE1cXV+8vMTCwsLIlJThHkO5urvgHjbhGzd/gYOEhonX2NiOkJLnHTnkHTjmHDjlHTjiHDfiHDdzdXelp6mytLWWmJqnqaqLjY99f4JrbXHg4ODV2Nrh4ePkHTiMjY/nHTnqHTm9vsAWGR5wcXRvb2+sra/j4+R+f4GGiIqKjI6trrBxc3WgoqWCg4aZm57IycqRkpSgoqS9vsCPkZPiHDe7vb3jHDgvLy/iHDe5ubnmHTfjHTfoGDjiHDaMkJDoHjriHDfkHTiFh4mQkJSbnZ+PkZOJi47c3d3e3t+vsLGgoqT5Hz7mGDzCxMWho6aIio2Bg4TKy82mqKqUlpjSFjf19fXrHjniHDjmHjnIyMqsrrDY2tqBg4WrrrHQ1NTk5OSYIcrwHjuZmpz+IUDIycrP0NHrHjr0Hzynqauw8T+IAAAAZXRSTlMAdgnMAzIGAgEE9h9RwXRJz/A6W5KZplOEz/j38GdDZRvLzf2I84QhcyPsc5PP9/N/G1no7u3S3ZV8fCgR6hdIvBAsRUGzgTlL9Hzelb9s4WIVw7Kv0rOZrhczzwm7XeOFhFY8h+zeNi4AAAGTSURBVCjPVZJZW9pAFIa/wCRnhgSUvaigArYqUCmrC5v7Wu2+L9r2AST2/9/2JKkY5+Kd7zlvZpKcGQBSwhkefdGrM2aePjmRLt28D8E8dhWhtxwKzj4Pv/TRqRTCHZZkLGeeAWu3f3WHI87HE4drlfeCgMVQAAaV2pUy0Z9M5YboInMeIQOBuSy/+80mW7Qjv5pAO3t5DhlKX87yrvgYZp2JCCHxM/37VGI9N1OHsaH/qEMSbQdZv30Hw5CtcumKqFW9bkm6Wr0ISsPAh0+s90f8Tcg1GzUg3WykmfVGjktfJkyBciH7YmnxduSx5rBQ6y2VJpv8Y5KwujA3v3Hmscpcj1QXTpkg6bZN6HoHCOh6wEdx32ZyKdyofHl6BEJoCSW8pxW0I8c/HJEU37rjInZju4iZOEiNNfTNB6+QzFvDPXNsKfsouZIc2Ja9BTW1sfFAs/N7dzFEU3YcWEl1tXst5evo10QqMTzs5pN31mE08T1qDaerJcxXn3nux3e04gFUvKiZiO/4rw+UUo8u0v/yP0PNNk8vPFYIAAAAAElFTkSuQmCC" alt="audi-logo-1995-download_optimized.png"/>  </body></html>   <span class="text-xl font-bold">  R055 & Sons.  <span class="text-blue-400">Car Care
                </span></span>  <!DOCTYPE html><html><head><meta charset="utf-8"><source
    type="image/webp"
    srcset="https://flagcdn.com/80x60/gb-sct.webp,
      https://flagcdn.com/160x120/gb-sct.webp 2x,
      https://flagcdn.com/240x180/gb-sct.webp 3x">
  <source
    type="image/png"
    srcset="https://flagcdn.com/80x60/gb-sct.png,
      https://flagcdn.com/160x120/gb-sct.png 2x,
      https://flagcdn.com/240x180/gb-sct.png 3x">
  <img
    src="https://flagcdn.com/80x60/gb-sct.png"
    width="30"
    height="40"
    alt="Scotland">
</picture><title>maserati-logo-2006-download_2_optimized.png</title></head><body><img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABkAAAAhCAMAAAAbHvCRAAAAyVBMVEVHcExZb411g5aQnKxVY3gAIE6nsb13f5Pe6fv///9HWHPe4+n+8PG0vMixusWosb6Fj58iLkqrtcKns8MbOmMAGkkQL1urtMHH0dnX3OKTo7Krs76cqbq/xs7Ax9AM/P////8MLln+/f39///++PlgdpIqR20GKVXyjpIPMVzvgYX0pagjQWhpf5xIYYPsaW784+TrS1AzUHTqVFr4w8budnuSoLN3jKb61teotscyVnvhERf5m53o7PD2s7ZcUm/mQ0n2trhVGjaFKpneAAAAH3RSTlMA/lmBKPyJAgP8Pvz9wrejPxXf+v77/XTq+plc+9TYs7DpUwAAAaRJREFUKM99U4mSoyAQRaMCiWYyueae6rTEJd7RmHOO7P7/Ry2ymmNSta8KGnj266ZtCGlBKWOMklvQH/YERki343S6enVNdL1PAPj0utcUI+YT8BrwZF5SyqMHHGGFyKF34UXZ/SMIACxdUPbx/pQiI8/oAmJ0kALBFc+tEyVWz11GKPJwK+Dr6PasJndGOsCjTMmpIULJoXNyekfu1qfHHKDKOb7RkxgglCvYHtQo1bqRo8T0VcaVhGyZQZQBct/UjA6DIGW+zMttVCmmCcTIHXCArzCUUoZhhGp31zD9molCWYWVDD9qpt8wnq7MSmSHUmx/12ot00eB6Pt+dJRqRrXrX8ZR+FhKbc9xnJ0xr/H951tbY+dohpKXzbSI4zgo9vsgjotiunlpbmq97tdzIzGSNNnMDSNN121J6TAdF3EQBwpqGqdD2v4eZzOZ/WoxmyROU2slN5rOzpi+tmJ13slk0Zwvzi66D4aB/Y9a2MHw3Afqk8FubC9q2OPR4LqtzFFq10hH5s9WtLy1utHas27blwwenIfBTV//5y3oFK/ez181PTjttrACVAAAAABJRU5ErkJggg==" alt="maserati-logo-2006-download_2_optimized.png"/></body><span style='font-size:45px;'>&#128513;</span></html>
            </div>
            
            <div class="hidden md:flex space-x-6">
                <a href="#home" class="hover:text-yellow-400 transition">Home</a>
                <a href="#services" class="hover:text-yellow-400 transition">Services</a>
                <a href="#gallery" class="hover:text-yellow-400 transition">Gallery</a>
                <a href="#about" class="hover:text-yellow-400 transition">About</a>
                <a href="#contact" class="hover:text-yellow-400 transition">Contact</a>
            </div>
            
            <button class="md:hidden text-white focus:outline-none" id="mobile-menu-button">
                <i class="fas fa-bars text-2xl"></i>
            </button>
        </div>
        
        <!-- Mobile menu -->
        <div class="md:hidden hidden bg-black py-2 px-4" id="mobile-menu">
            <a href="#home" class="block py-2 hover:text-yellow-400 transition">Home</a>
            <a href="#services" class="block py-2 hover:text-yellow-400 transition">Services</a>
            <a href="#gallery" class="block py-2 hover:text-yellow-400 transition">Gallery</a>
            <a href="#about" class="block py-2 hover:text-yellow-400 transition">About</a>
            <a href="#contact" class="block py-2 hover:text-yellow-400 transition">Contact</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-image h-screen flex items-center justify-center text-white">
        <div class="text-center px-4">
            <h1 class="text-4xl md:text-6xl font-bold mb-4"><span class="shine-text"><span class="text-blue-400">Premium Car Care</span></h1><span class="text-blue-400">
            <p class="text-xl md:text-2xl mb-8"><span class="shine-text">Why choose R055 and Sons?.<p> Let me restore your car to showroom shine with our professional Car Cleaning services in West Belfast,Drop your car off and pick it up.</p>
            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <a href="#contact" class="bg-yellow-400 hover:bg-yellow-500 text-black font-bold py-3 px-8 rounded-full transition duration-300 inline-block">
                    Book Now
                </a>
                <a href="tel:07801959777" class="bg-transparent border-2 border-white hover:bg-white hover:text-black text-white font-bold py-3 px-8 rounded-full transition duration-300 inline-block">
                    <i class="fas fa-phone mr-2"></i> Call Us
                </a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-16 bg-gray-100">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold mb-2">Our <span class="text-yellow-500">Services</span></h2>
                <p class="text-gray-600 max-w-2xl mx-auto">We offer a car wash and vaccum service to keep your vehicle looking its best</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Service 1 -->
                <div class="service-card bg-white rounded-lg overflow-hidden shadow-md transition duration-300">
                    <div class="h-48 bg-gray-300 flex items-center justify-center">
                        <i class="fas fa-spray-can text-6xl text-yellow-500"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Exterior washing</h3>
                        <p class="text-gray-600 mb-4">Complete exterior wash,polish and restore your paint's shine and protect it from the elements.</p>
                        <div class="flex justify-between items-center">
                            <p class="text-yellow-500 font-bold">From £49</p>
                            <a href="#contact" class="text-sm text-yellow-500 hover:text-yellow-600 font-medium">Book Now <i class="fas fa-arrow-right ml-1"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Service 2 -->
                <div class="service-card bg-white rounded-lg overflow-hidden shadow-md transition duration-300">
                    <div class="h-48 bg-gray-300 flex items-center justify-center">
                        <i class="fas fa-couch text-6xl text-yellow-500"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Interior cleaning</h3>
                        <p class="text-gray-600 mb-4">Deep cleaning of all surfaces, leather treatment, odor removal, and UV protection for a fresh and clean interior.</p>
                        <div class="flex justify-between items-center">
                            <p class="text-yellow-500 font-bold">From £49</p>
                            <a href="#contact" class="text-sm text-yellow-500 hover:text-yellow-600 font-medium">Book Now <i class="fas fa-arrow-right ml-1"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Service 3 -->
                <div class="service-card bg-white rounded-lg overflow-hidden shadow-md transition duration-300">
                    <div class="h-48 bg-gray-300 flex items-center justify-center">
                        <i class="fas fa-star text-6xl text-yellow-500"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3">Full car washing Package</h3>
                        <p class="text-gray-600 mb-4">Complete interior and exterior cleaning.</p>
                        <div class="flex justify-between items-center">
                            <p class="text-yellow-500 font-bold">From £99</p>
                            <a href="#contact" class="text-sm text-yellow-500 hover:text-yellow-600 font-medium">Book Now <i class="fas fa-arrow-right ml-1"></i></a>
                        </div>
                    </div>
                </div>
                
                <!-- Service 4 -->
                <div class="service-card bg-white rounded-lg overflow-hidden shadow-md transition duration-300">
                    <div class="h-48 bg-gray-300 flex items-center justify-center">
                        <i class="fas fa-tint text-6xl text-yellow-500"></i>
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-bold mb-3"></h3>
                        <p class="text-gray-600 mb-4">Advanced paint protection that lasts for years with hydrophobic properties that repel water, dirt, and contaminants.</p>
                        <div class="flex justify-between items-center">
                            <p class="text-yellow-500 font-bold"></p>
                            <a href="#contact" class="text-sm text-yellow-500 hover:text-yellow-600 font-medium">Book Now <i class="fas fa-arrow-right ml-1"></i></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Gallery Section -->
    <section id="gallery" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold mb-2">Our <span class="text-yellow-500">Work</span></h2>
                <p class="text-gray-600 max-w-2xl mx-auto">See the transformation we can achieve with your vehicle</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-12">
                <!-- Before/After 1 -->
                <div class="before-after rounded-lg overflow-hidden shadow-lg">
                    <img src="https://images.unsplash.com/photo-1607860108855-64acf2078ed9?ixlib=rb-4.0.3" alt="Dirty car">
                    <div class="after">
                       
                    </div>
                    
                </div>
                
                <!-- Before/After 2 -->
                
                    </div>
                    <div class="slider"></div>
                </div>
            </div>
            
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                <div class="relative group overflow-hidden rounded-lg shadow-md hover:shadow-lg transition duration-300">
                    <img src="https://images.unsplash.com/photo-1605559424843-9e4c228bf1c2?ixlib=rb-4.0.3" alt="Clean car" class="w-full h-48 object-cover">
                    <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                        <i class="fas fa-search-plus text-white text-2xl"></i>
                    </div>
                </div>
                <div class="relative group overflow-hidden rounded-lg shadow-md hover:shadow-lg transition duration-300">
                    
                        <i class="fas fa-search-plus text-white text-2xl"></i>
                    </div>
                </div>
                <div class="relative group overflow-hidden rounded-lg shadow-md hover:shadow-lg transition duration-300">
                    <img src="https://images.unsplash.com/photo-1492144534655-ae79c964c9d7?ixlib=rb-4.0.3" alt="Shiny car" class="w-full h-48 object-cover">
                    <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                        <i class="fas fa-search-plus text-white text-2xl"></i>
                    </div>
                </div>
                <div class="relative group overflow-hidden rounded-lg shadow-md hover:shadow-lg transition duration-300">
                    <img src="https://images.unsplash.com/photo-1502877338535-766e1452684a?ixlib=rb-4.0.3" alt="Detailing process" class="w-full h-48 object-cover">
                    <div class="absolute inset-0 bg-black bg-opacity-50 flex items-center justify-center opacity-0 group-hover:opacity-100 transition duration-300">
                        <i class="fas fa-search-plus text-white text-2xl"></i>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-16 bg-gray-800 text-white">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row items-center">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pr-8">
                    <h2 class="text-3xl font-bold mb-6">About <span class="text-yellow-400">R055 & Sons.</span></h2>
                    <p class="mb-4">Founded in 2025,R055 & Sons has been providing premium car care services to thousands of satisfied customers in Belfast and surrounding areas. Our mission is to restore your vehicle to its original showroom condition using the latest techniques and highest quality products.</p>
                    <p class="mb-4">The staff are extensively trained and certified in the latest detailing. We use only professional-grade equipment and eco-friendly products that are safe for your vehicle and the environment.</p>
                    <div class="flex flex-wrap gap-3 mt-6">
                        <div class="bg-yellow-400 text-black px-4 py-2 rounded-full font-bold flex items-center">
                            <i class="fas fa-award mr-2"></i> Certified
                        </div>
                        <div class="bg-yellow-400 text-black px-4 py-2 rounded-full font-bold flex items-center">
                            <i class="fas fa-leaf mr-2"></i> Eco-Friendly
                        </div>
                        <div class="bg-yellow-400 text-black px-4 py-2 rounded-full font-bold flex items-center">
                            <i class="fas fa-thumbs-up mr-2"></i> 100% Satisfaction
                        </div>
                    </div>
                </div>
                <div class="md:w-1/2">
                    <div class="bg-gray-700 p-6 rounded-lg shadow-lg">
                        <h3 class="text-xl font-bold mb-4 text-yellow-400">Why Choose Us?</h3>
                        <ul class="space-y-3">
                            <li class="flex items-start">
                                <i class="fas fa-check text-yellow-400 mt-1 mr-2"></i>
                                <span>5+ years of experience in professional detailing</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check text-yellow-400 mt-1 mr-2"></i>
                                <span>100% satisfaction guarantee on all our services</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check text-yellow-400 mt-1 mr-2"></i>
                                <span>Mobile detailing service available at your location</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check text-yellow-400 mt-1 mr-2"></i>
                                <span>Premium products that provide longer-lasting results</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check text-yellow-400 mt-1 mr-2"></i>
                                <span>Flexible scheduling including evenings and weekends</span>
                            </li>
                            <li class="flex items-start">
                                <i class="fas fa-check text-yellow-400 mt-1 mr-2"></i>
                                <span>Competitive pricing with no hidden fees</span>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="py-16 bg-gray-100">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold mb-2">Customer <span class="text-yellow-500">Testimonials</span></h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Don't just take our word for it - hear what our customers have to say</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Testimonial 1 -->
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-300 flex items-center justify-center mr-4 overflow-hidden">
                            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Michael R." class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Michael R.</h4>
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-700">"My 10-year-old BMW looks brand new after the full detailing package. The team at R055's did an incredible job removing years of swirl marks and stains. The interior smells fresh and the paint has a deep shine I haven't seen since I bought the car!"</p>
                </div>
                
                <!-- Testimonial 2 -->
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-300 flex items-center justify-center mr-4 overflow-hidden">
                            <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="Sarah L." class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">Sarah L.</h4>
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-700">"Worth every penny. My car stays cleaner longer and water just beads right off. Excellent service and attention to detail. They even cleaned areas I didn't know existed! Will definitely be coming back for regular maintenance."</p>
                </div>
                
                <!-- Testimonial 3 -->
                <div class="bg-white p-6 rounded-lg shadow-md">
                    <div class="flex items-center mb-4">
                        <div class="w-12 h-12 rounded-full bg-gray-300 flex items-center justify-center mr-4 overflow-hidden">
                            <img src="https://randomuser.me/api/portraits/men/75.jpg" alt="James T." class="w-full h-full object-cover">
                        </div>
                        <div>
                            <h4 class="font-bold">James T.</h4>
                            <div class="flex text-yellow-400">
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                                <i class="fas fa-star"></i>
                            </div>
                        </div>
                    </div>
                    <p class="text-gray-700">"I've tried several Car Washers in the Belfast area and R055 and Sons is by far the best. They removed coffee stains from my seats that I thought were permanent. The headlight restoration made my car look years newer. Professional service from start to finish."</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-16 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-12">
                <h2 class="text-3xl font-bold mb-2">Get In <span class="text-yellow-500">Touch</span></h2>
                <p class="text-gray-600 max-w-2xl mx-auto">Ready to give your car the treatment it deserves? Contact us today</p>
            </div>
            
            <div class="flex flex-col md:flex-row">
                <div class="md:w-1/2 mb-8 md:mb-0 md:pr-8">
                    <div class="bg-gray-100 p-6 rounded-lg shadow-md h-full">
                        <h3 class="text-xl font-bold mb-4">Contact Information</h3>
                        <div class="space-y-4">
                            <div class="flex items-start">
                                <i class="fas fa-map-marker-alt text-yellow-500 mt-1 mr-3"></i>
                                <div>
                                    <h4 class="font-bold">Address</h4>
                                    <p>TBC</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <i class="fas fa-phone-alt text-yellow-500 mt-1 mr-3"></i>
                                <div>
                                    <h4 class="font-bold">Phone</h4>
                                    <p>+447801 959777</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <i class="fas fa-envelope text-yellow-500 mt-1 mr-3"></i>
                                <div>
                                    <h4 class="font-bold">Email</h4>
                                    <p>r055mcclure@hotmail.co.uk</p>
                                </div>
                            </div>
                            <div class="flex items-start">
                                <i class="fas fa-clock text-yellow-500 mt-1 mr-3"></i>
                                <div>
                                    <h4 class="font-bold">Hours</h4>
                                    <p>Monday - Friday: 8am - 6pm<br>Saturday: 9am - 4pm<br>Sunday: Closed</p>
                                </div>
                            </div>
                        </div>
                        
                        <div class="mt-6">
                            <h3 class="text-xl font-bold mb-4">Follow Us</h3>
                            <div class="flex space-x-4">
                                <a href="#" class="bg-gray-700 text-white w-10 h-10 rounded-full flex items-center justify-center hover:bg-yellow-500 transition">
                                    <i class="fab fa-facebook-f"></i>
                                </a>
                                
                                </a>
                                
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="md:w-1/2">
                    <div class="bg-gray-100 p-6 rounded-lg shadow-md">
                        <h3 class="text-xl font-bold mb-4">Book An Appointment</h3>
                        <form id="booking-form">
                            <div class="mb-4">
                                <label for="name" class="block font-medium mb-1">Name *</label>
                                <input type="text" id="name" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500" required>
                            </div>
                            <div class="mb-4">
                                <label for="email" class="block font-medium mb-1">Email *</label>
                                <input type="email" id="email" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500" required>
                            </div>
                            <div class="mb-4">
                                <label for="phone" class="block font-medium mb-1">Phone *</label>
                                <input type="tel" id="phone" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500" required>
                            </div>
                            <div class="mb-4">
                                <label for="service" class="block font-medium mb-1">Service *</label>
                                <select id="service" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500" required>
                                    <option value="">Select a service</option>
                                    <option value="exterior">Exterior Detailing</option>
                                    <option value="interior">Interior Detailing</option>
                                    <option value="full">Full Detailing Package</option>
                                    
                                </select>
                            </div>
                            <div class="mb-4">
                                <label for="date" class="block font-medium mb-1">Preferred Date *</label>
                                <input type="date" id="date" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500" required>
                            </div>
                            <div class="mb-4">
                                <label for="message" class="block font-medium mb-1">Special Requests</label>
                                <textarea id="message" rows="3" class="w-full px-4 py-2 border rounded-lg focus:outline-none focus:ring-2 focus:ring-yellow-500"></textarea>
                            </div>
                            <button type="submit" class="bg-yellow-500 hover:bg-yellow-600 text-black font-bold py-3 px-6 rounded-lg transition duration-300 w-full">
                                Submit Booking
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black text-white py-8">
        <div class="container mx-auto px-4">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="mb-4 md:mb-0">
                    <div class="flex items-center">
                        </i>
                        <span class="text-xl font-bold">R.McClure & Sons.<span class="text-blue-400"> Car Care</span></span>
                    </div>
                    <p class="mt-2 text-gray-400">Premium Car Care services in Belfast</p>
                </div>
                
                <div class="flex flex-col items-center md:items-end">
                    <div class="flex space-x-4 mb-4">
                        <a href="#" class="text-gray-400 hover:text-yellow-400 transition">
                          <i class="fab fa-facebook"></i>  
                        </a>
                        
                        </a>
                       
                        </a>
                    </div>
                    <p class="text-gray-400 text-sm">&copy; 2025 R.McClure All rights reserved.</p>
              
           
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });
        
        // Before/After slider functionality
        document.querySelectorAll('.before-after').forEach(slider => {
            const after = slider.querySelector('.after');
            const sliderHandle = slider.querySelector('.slider');
            let isDragging = false;
            
            function moveSlider(e) {
                if (!isDragging) return;
                
                let x;
                if (e.type === 'mousemove') {
                    x = e.pageX - slider.getBoundingClientRect().left;
                } else if (e.type === 'touchmove') {
                    x = e.touches[0].pageX - slider.getBoundingClientRect().left;
                }
                
                const sliderWidth = slider.offsetWidth;
                let percentage = (x / sliderWidth) * 100;
                
                // Limit between 0 and 100
                percentage = Math.max(0, Math.min(100, percentage));
                
                after.style.width = ${percentage}%;
                sliderHandle.style.left = ${percentage}%;
            }
            
            sliderHandle.addEventListener('mousedown', () => {
                isDragging = true;
            });
            
            slider.addEventListener('mousemove', moveSlider);
            
            document.addEventListener('mouseup', () => {
                isDragging = false;
            });
            
            // Touch support
            sliderHandle.addEventListener('touchstart', () => {
                isDragging = true;
            });
            
            slider.addEventListener('touchmove', moveSlider);
            
            document.addEventListener('touchend', () => {
                isDragging = false;
            });
        });
        
        // Form submission
        document.getElementById('booking-form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Get form values
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const phone = document.getElementById('phone').value;
            const service = document.getElementById('service').value;
            const date = document.getElementById('date').value;
            const message = document.getElementById('message').value;
            
            // Simple validation
            if (!name || !email || !phone || !service || !date) {
                alert('Please fill in all required fields');
                return;
            }
            
            // In a real app, you would send this data to your server
            alert(Thanks ${name}! Your ${service} booking request for ${date} has been received. We'll contact you shortly at ${phone} or ${email} to confirm.);
            
            // Reset form
            this.reset();
        });
        
        // Smooth scrolling for navigation
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    document.getElementById('mobile-menu').classList.add('hidden');
                }
            });
        });
    </script>
</body>
</html>
