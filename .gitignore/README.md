using System;

namespace first_space
{
    /* here  first_space is a namespacename  */

    class namespace_cl
    {
        //namespace_c1 is a className

        public void func()
            //func is a method
        {
            Console.WriteLine("Inside first_space");
        }
    }
}

namespace second_space
{

    class namespace_cl
    {

        public void func()
        {
            Console.WriteLine("Inside second_space");
        }
    }
}

class TestClass
{

    static void Main(string[] args)
    {
        first_space.namespace_cl fc = new first_space.namespace_cl();//object creation for first namespace
        second_space.namespace_cl sc = new second_space.namespace_cl();//object creation for second namespace 
        fc.func();
        sc.func();
        Console.ReadKey();
    }
}
