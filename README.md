
<script>
// javascript program to convert 12 hour
// format to 24 hour format


function print24(str)
{
	// Get hours
	var h1 = Number(str[1] - '0');
	var h2 = Number(str[0] - '0');
	var hh = (h2 * 10 + h1 % 10);

	// If time is in "AM"
	if (str[8] == 'A')
	{
		if (hh == 12)
		{
               let j = 6;
               let k  =7;
           var res = str[k].concat[j];
           if(res<15){
                res  = res + 45;
              str[j]  = res[0];
               str[k]  = res[1];
            }
            else{
              var m =0;
                var res2 = 60-(res+45);
                 if(res2<9){var res3 = m.concat(str[j])
                 str[j] = res3[0];
                 str[k] = res3[1];
                 }
                 else{
                 str[j] = res2[0];
                 str[k] = res2[1];
                 }
                 str[j-2] = str[j-2]+1;
             }
			document.write("00");
            if(str[]
			for (var i = 2; i <= 7; i++)
				document.write(str[i]);
		}
		else
		{
			for (var i = 0; i <= 7; i++)
				document.write(str[i]);
		}
	}

	// If time is in "PM"
	else
	{
		if (hh == 12)
		{
			document.write("12");
			for (var i = 2; i <= 7; i++)
				document.write(str[i]);
		}
		else
		{
			hh = hh + 12;
			document.write(hh);
			for (var i = 2; i <= 7; i++)
				document.write(str[i]);
		}
	}
}

// Driver code

	var str = "07:05:45PM";
	print24(str);
</script>
