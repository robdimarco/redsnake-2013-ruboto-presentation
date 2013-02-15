!SLIDE bullets
# Getting Warmed Up
## Android SDK + JRuby => Ruboto

!SLIDE bullets incremental
# Android Basics #

 * Java-based SDK
 * Byte code compiled into Dalvik executables
 * Code, data, and resources packaged in APK

!SLIDE bullets incremental
# Android Components #

 * Activities (single screen)
 * Services (background process)
 * Content Providers (data management)
 * Broadcast Receivers (receives system messages)
 * Manifest file

!SLIDE smaller
# Example Activity  #

    @@@java
		// JDK classes
		import java.util.ArrayList;
		// Android API
		import android.app.Activity;
		import android.content.Context;
		import android.os.Bundle;
		import android.support.v4.view.ViewPager; // Local code
		
		public class ActionBarTabsPager extends Activity {
		    ViewPager mViewPager;
		    TabsAdapter mTabsAdapter;

		    @Override
		    // Callback
		    protected void onCreate(Bundle savedInstanceState) {
		        super.onCreate(savedInstanceState);

		        mViewPager = new ViewPager(this);
		        mViewPager.setId(R.id.pager);
		        setContentView(mViewPager);
		    }
		}

!SLIDE bullets incremental
# JRuby

* 100% Java implementation of Ruby
* Most of the Ruby Standard Lib, 1.9 compatible
* Easy integration with Ruby and Java

!SLIDE smaller
# Example JRuby code

    @@@ruby
		
		i = java.lang.Integer::MAX_VALUE
		# 2147483647
		
		a = java.util.ArrayList.new
		# #<Java::JavaUtil::ArrayList:0x111bda67>
		
		a << "1"
		# #<Java::JavaUtil::ArrayList:0x111bda67>
		
		a << 2
		# #<Java::JavaUtil::ArrayList:0x111bda67>
		
		a.map(&:to_i).reduce(&:+)
		# 3

		require 'path/to/mycode.jar'
		
!SLIDE center
# Beautiful Ruby, Practical JVM

![Beauty And The Geek](beauty_and_the_geek.png)

