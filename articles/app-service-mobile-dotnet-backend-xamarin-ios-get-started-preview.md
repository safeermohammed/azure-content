<properties
	pageTitle="Get Started with Mobile Apps in Xamarin iOS"
	description="Get started using Xamarin iOS to build an Azure Mobile App with Azure App Service."
	services="app-service\mobile"
	documentationCenter="xamarin"
	authors="christopheranderson"
	manager="dwrede"
	editor=""/>

<tags
	ms.service="app-service-mobile"
	ms.workload="mobile"
	ms.tgt_pltfrm="mobile-xamarin-ios"
	ms.devlang="dotnet"
	ms.topic="hero-article"
	ms.date="02/24/2015"
	ms.author="chrande"/>


# <a name="getting-started"> </a>Create a Xamarin iOS app

[AZURE.INCLUDE [app-service-mobile-selector-get-started-preview](../includes/app-service-mobile-selector-get-started-preview.md)]

This tutorial shows you how to add a cloud-based backend service to a Xamarin iOS app with Azure Mobile App. In this tutorial, you will create both a new .NET service and a simple _To do list_ app that stores app data in the .NET backend.



## Create a new mobile app backend

[AZURE.INCLUDE [app-service-mobile-dotnet-backend-create-new-service-preview](../includes/app-service-mobile-dotnet-backend-create-new-service-preview.md)]

## Create a new Xamarin iOS app

Once you have created your mobile app backend, you can follow an easy quickstart in the Azure Portal to either create a new app or modify an existing app to connect to your mobile app backend.

In this section you will download a new Xamarin iOS app and a service project for your mobile app backend.

1. In the Azure Portal, click **Mobile App**, and then click the mobile app backend that you just created.

2. At the top of the blade, click **Add Client** and expand **Xamarin iOS**.

	![][6]

	This displays the three easy steps to create a Xamarin iOS app connected to your mobile app backend.

3. If you haven't already done so, download and install <a href="https://go.microsoft.com/fwLink/p/?LinkID=257546" target="_blank">Visual Studio Professional 2013</a> on your local computer or virtual machine.  

4. Download and install [Xcode] v4.4 or a later version and [Xamarin Studio]. You can also use Xamarin for Visual Studio.

5. Under **Download and publish your service to the cloud**, click **Download**.

 This downloads a solution contains projects for both the mobile app backend and for the sample _To do list_ application that is connected to your mobile app backend. Save the compressed project file to your local computer, and make a note of where you save it.

6. Download your publish profile, save the downloaded file to your local computer, and make a note of where you save it.

## Test the mobile app backend

[AZURE.INCLUDE [app-service-mobile-dotnet-backend-test-local-service-preview](../includes/app-service-mobile-dotnet-backend-test-local-service-preview.md)]

## Publish your mobile app backend

[AZURE.INCLUDE [app-service-mobile-dotnet-backend-publish-service-preview](../includes/app-service-mobile-dotnet-backend-publish-service-preview.md)]

## Run the Xamarin iOS app

The final stage of this tutorial is to build and run your new app.

1. Navigate to the client project within the mobile app backend solution, in either Visual Studio or Xamarin Studio.

	![][8]

	![][9]

2. Press the **Run** button to build the client project and start the app in the iPhone emulator.

3. In the app, type meaningful text, such as _Complete the tutorial_ and then click the plus (**+**) icon.

	![][10]

	This sends a POST request to the new mobile app backend hosted in Azure. Data from the request is inserted into the TodoItem table. Items stored in the table are returned by the mobile app backend, and the data is displayed in the list.

>[AZURE.NOTE]You can review the code that accesses your mobile app backend to query and insert data in the QSTodoService.cs C# file.


<!-- Anchors. -->
[Getting started with mobile app backends]:#getting-started
[Create a new mobile app backend]:#create-new-service
[Next Steps]:#next-steps



<!-- Images. -->
[6]: ./media/app-service-mobile-dotnet-backend-xamarin-ios-get-started-preview/xamarin-ios-quickstart.png
[8]: ./media/app-service-mobile-dotnet-backend-xamarin-ios-get-started-preview/mobile-xamarin-project-ios-vs.png
[9]: ./media/app-service-mobile-dotnet-backend-xamarin-ios-get-started-preview/mobile-xamarin-project-ios-xs.png
[10]: ./media/app-service-mobile-dotnet-backend-xamarin-ios-get-started-preview/mobile-quickstart-startup-ios.png

<!-- URLs. -->
[Get started with offline data sync]: /en-us/documentation/articles/app-service-mobile-xamarin-ios-get-started-offline-data-preview
[Get started with authentication]: /en-us/documentation/articles/app-service-mobile-dotnet-backend-xamarin-ios-get-started-preview-users
[Get started with push notifications]: /en-us/documentation/articles/app-service-mobile-dotnet-backend-xamarin-ios-get-started-preview-push
[Visual Studio Professional 2013]: https://go.microsoft.com/fwLink/p/?LinkID=257546
[Mobile app SDK]: http://go.microsoft.com/fwlink/?LinkId=257545
[Azure Portal]: https://portal.azure.com/
[JavaScript backend version]: /en-us/documentation/articles/partner-xamarin-mobile-services-ios-get-started
[Get started with data in app services using Visual Studio 2012]: /en-us/documentation/articles/app-service-mobile-windows-store-dotnet-get-started-data-vs2012-preview
[Troubleshoot a mobile app .NET backend]: /en-us/documentation/articles/app-service-mobile-dotnet-backend-how-to-troubleshoot-preview


[Xamarin Studio]: http://xamarin.com/download
[Xcode]: https://go.microsoft.com/fwLink/?LinkID=266532&clcid=0x409
[Xamarin for Windows]: https://go.microsoft.com/fwLink/?LinkID=330242&clcid=0x409
