CLASSPATH=@TOOLS_CLASSPATH@:@ANT_CLASSPATH@

all-local:
	@echo "Building Dependencies"
	cd @top_srcdir@/jdepends && @JAVA@ -Xmx128m -Xms64m -Xss1024k -classpath "$(CLASSPATH)" -Dant.home="@ANT_HOME@" -Dbuild_dir="@abs_top_builddir@" org.apache.tools.ant.launch.Launcher $(ANT_VERBOSE) -f build.xml build
