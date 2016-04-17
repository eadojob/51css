# 51css
> link: https://raw.githubusercontent.com/eadojob/51css/master/base.css

```
<?php 
$Base = new Base();
$Base->run();
class Base
{
	private $css    = "";
	private $colors = 
			[
				['000'    , '#000'   ],  
				['333'    , '#333'   ],  
				['555'    , '#555'   ],  
				['777'    , '#777'   ],  
				['fff'    , '#fff'   ],  
				['ccc'    , '#ccc'   ],  
				['ebebeb' , '#ebebeb'],
				['dcdcdc' , '#dcdcdc'],
				['f5f5f5' , '#f5f5f5'],
				['red'    , 'red'    ],
				['green'  , 'green'  ],
				['blue'   , 'blue'   ],
				['primary', '#337ab7'],
				['success', '#5cb85c'],
				['info'   , '#5bc0de'],
				['warning', '#f0ad4e'],
				['danger' , '#d9534f'],
			];

	public function run()
	{
		// weight height line-height
		for ($i=1;$i<=100;$i++)
        {
            $this->css.=".w".$i."{width:".$i."%;}";
        }
		echo $this->css;echo "<br/>";$this->css="";

		for ($i=1;$i<=100;$i++)
        {
            $this->css.=".h".$i."{height:".$i."%;}";
        }
		echo $this->css;echo "<br/>";$this->css="";

		for ($i=1;$i<=1500;$i++)
        {
            $this->css.=".w-".$i."{width:".$i."px;}";
        }
		echo $this->css;echo "<br/>";$this->css="";

		for ($i=1;$i<=1500;$i++)
        {
            $this->css.=".h-".$i."{height:".$i."px;}";
        }
		echo $this->css;echo "<br/>";$this->css="";

		for ($i=1;$i<=100;$i++)
        {
            $this->css.=".l-h-".$i."{line-height:".$i."px;}";
        }
		echo $this->css;echo "<br/>";$this->css="";

		// font-size
		for ($i=1;$i<=100;$i++)
        {
            $this->css.=".f-".$i."{font-size:".$i."px;}";
        }
		echo $this->css;echo "<br/>";$this->css="";

		// font-weight
		echo ".f-w-b{font-weight: bold;}.f-w-n{font-weight: normal;}";
		echo "<br/>";

		// font-family
		echo ".yahei{font-family:'microsoft yahei';}.arial{font-family:'arial';}.simsun{font-family:'simsun';}.simhei{font-family:'simhei';}.sans-serif{font-family:'sans-serif';}";
		echo "<br/>";

		// margin
		echo ".m-auto{margin:0 auto;}";
		echo "<br/>";

		for ($i=1;$i<=100;$i++)
		{
			$this->css .= ".m-" . $i . "{margin:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		for ($i=1;$i<=100;$i++)
		{
			$this->css .= ".m-l-" . $i . "{margin-left:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		for ($i=1;$i<=100;$i++)
		{
			$this->css .= ".m-r-" . $i . "{margin-right:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		for ($i=1;$i<=100;$i++)
		{
			$this->css .= ".m-t-" . $i . "{margin-top:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		for ($i=1;$i<=100;$i++)
		{
			$this->css .= ".m-b-" . $i . "{margin-bottom:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";

		// padding
		for ($i=1;$i<=100;$i++)
		{
			$this->css .= ".p-" . $i . "{padding:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		for ($i=1;$i<=100;$i++)
		{
			$this->css .= ".p-l-" . $i . "{padding-left:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		for ($i=1;$i<=100;$i++)
		{
			$this->css .= ".p-r-" . $i . "{padding-right:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		for ($i=1;$i<=100;$i++)
		{
			$this->css .= ".p-t-" . $i . "{padding-top:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		for ($i=1;$i<=100;$i++)
		{
			$this->css .= ".p-b-" . $i . "{padding-bottom:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";

		// border
		echo ".border{border:1px solid #ebebeb;}.noborder{border: 0px;}";
		echo "<br/>";
		// border-width
		for ($i=1;$i<=30;$i++)
		{
			$this->css .= ".border-" . $i . "{border-width:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		for ($i=1;$i<=30;$i++)
		{
			$this->css .= ".border-left-" . $i . "{border-left-width:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		for ($i=1;$i<=30;$i++)
		{
			$this->css .= ".border-right-" . $i . "{border-right-width:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		for ($i=1;$i<=30;$i++)
		{
			$this->css .= ".border-top-" . $i . "{border-top-width:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		for ($i=1;$i<=30;$i++)
		{
			$this->css .= ".border-bottom-" . $i . "{border-bottom-width:" . $i . "px;}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		// border-color
		foreach ($this->colors as $v)
		{
			$this->css .= ".border-" . $v[0] . "{border-color:" . $v[1] . ";}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		foreach ($this->colors as $v)
		{
			$this->css .= ".border-l-" . $v[0] . "{border-left-color:" . $v[1] . ";}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		foreach ($this->colors as $v)
		{
			$this->css .= ".border-r-" . $v[0] . "{border-right-color:" . $v[1] . ";}";
		}
		echo $this->css;echo "<br/>";$this->css="";
		foreach ($this->colors as $v)
        {
            $this->css .= ".border-t-" . $v[0] . "{border-top-color:" . $v[1] . ";}";
        }
		echo $this->css;echo "<br/>";$this->css="";
		foreach ($this->colors as $v)
        {
            $this->css .= ".border-b-" . $v[0] . "{border-bottom-color:" . $v[1] . ";}";
        }
		echo $this->css;echo "<br/>";$this->css="";

		// color
		foreach ($this->colors as $v)
        {
            $this->css .= ".c-" . $v[0] . "{color:" . $v[1] . ";}";
        }
		echo $this->css;echo "<br/>";$this->css="";

		// background-color
		foreach ($this->colors as $v)
        {
            $this->css .= ".bgc-" . $v[0] . "{background-color:" . $v[1] . ";}";
        }
		echo $this->css;echo "<br/>";$this->css="";

		// a
		echo ".a-none{text-decoration:none !important;}";
		echo $this->css;echo "<br/>";$this->css="";

		foreach ($this->colors as $v)
        {
            $this->css .= ".a-" . $v[0] . "{color:" . $v[1] . " !important;}";
        }
		echo "<br/>";$this->css="";

		// float
		echo ".fl{float:left;}.fr{float:right;}.clear{clear:both;}";
		echo "<br/>";

		// text-align
		echo ".left{text-align:left;}.right{text-align:right;}.center{text-align:center;}.v-middle{vertical-align:middle;}.v-top{vertical-align:top;}.v-bottom{vertical-align:bottom;}";
		echo "<br/>";

		// cursor radius noradius shadow noshadow
		echo ".cursor{cursor:pointer;}.radius{border-radius:4px;}.noradius{border-radius:0;}.shadow{box-shadow:0 0 8px #d0d0d0;}.noshadow{box-shadow: 0 0 0;}";
		echo "<br/>";

		// line
		echo ".line-deshed{border-bottom:1px dashed #ebebeb;}.line-solid{border-bottom:1px solid #ebebeb;}.sep{margin:0 4px;color:#dcdcdc;}";
		echo "<br/>";

		// form
		echo "input[type='text'],input[type='password'],textarea,select{padding:2px 4px;font-size:14px;border-radius:4px;border:1px solid #ebebeb;-webkit-transition:box-shadow 0.30s ease-in-out;-moz-transition:box-shadow 0.30s ease-in-out;}input[type='text']:focus,input[type='password']:focus,textarea:focus,select:focus{outline:none;border:#87C6F9 1px solid;box-shadow: 0 0 8px rgba(103,166,217,1);}input[type='button'],input[type='submit'],input[type='reset']{padding: 2px 4px;font-size: 14px;border-radius: 4px;border: 0;color: #fff;cursor: pointer;}input[type='button']:hover,input[type='submit']:hover,input[type='reset']:hover{opacity: 0.96;}";
		echo "<br/>";
		echo ".button{padding:8px 12px;color:#fff;border-radius:2px;background-color:#f5f5f5;text-decoration:none;font-size:14px;font-family:simhei;cursor:pointer;}.button:hover{color:#fff;text-decoration:none;opacity:0.9;-webkit-opacity:0.9;-moz-opacity:0.9;-khtml-opacity:0.9;filter:alpha(opacity=90);-ms-filter:'progid:DXImageTransform.Microsoft.Alpha(Opacity=90)';filter:progid:DXImageTransform.Microsoft.Alpha(Opacity=90);}.button:active,.button:link,.button:visited{text-decoration:none;color:#fff;}.button-sm{padding:6px 10px;font-size:12px;}.button-md{padding:8px 12px;font-size:14px;}.button-lg{padding:12px 16px;font-size:16px;}";  
		echo "<br/>";

	}//function end

}//class end
```
